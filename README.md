
[![Build Status](https://secure.travis-ci.org/Nodeclipse/org.nodeclipse.gitaddon.png)](http://travis-ci.org/Nodeclipse/org.nodeclipse.gitaddon)
<a href="http://marketplace.eclipse.org/marketplace-client-intro?mpc_install=1076754" title="Drag and drop into a running Eclipse to install Nodeclipse Git Addon">
  <img src="http://marketplace.eclipse.org/sites/all/modules/custom/marketplace/images/installbutton.png"/>
</a>

## About

Associate `*.git*` files with TextEditor

![](gitaddon.core/help/with-git-addon.PNG)

Builded against Indigo and tested in Kepler.

      <editor
            class="org.eclipse.ui.editors.text.TextEditor"
            contributorClass="org.eclipse.ui.texteditor.BasicTextEditorActionContributor"
            default="true"
            extensions="gitignore,gitmodules,gitattributes"
            icon="icons/git.ico"
            id="org.eclipse.ui.DefaultTextEditor"
            name="Text Editor">
      </editor>

## Why

I got tired of Eclipse opening .gitignore in external Editor and Eclipse crashes when changing files associations.  
~~[Bug 412518 - Changing file associations causes Eclipse Kepler to crash (was .gitignore value causes Eclipse crash)](https://bugs.eclipse.org/bugs/show_bug.cgi?id=412518)~~

## Get

1. In Eclipse import.. Git
2. as New general project 
3. right-click import Existing Maven projects

## Install from sources

1. `mvn package`  
2. `npm install http-server -g`  
3. `http-server gitaddon.site\target\repository -p 8010`
4. start http://localhost:8010/  
5. // navigate `http://localhost:8010/` in browser to check  
5. Help->Install New Software, enter http://localhost:8010/ in Work With  

Run offline if to re-build
`mvn -o package`

## Ideas

check [issues](https://github.com/Nodeclipse/org.nodeclipse.gitaddon/issues)

## Created

Created with Open-Archetypes

http://code.google.com/p/open-archetypes/

`mvn archetype:generate -DarchetypeCatalog=http://open-archetypes.github.io/maven-repo/snapshots/`

or with Eclipse

read https://github.com/open-archetypes/tycho-eclipse-plugin-archetype

![](with-eclipse.png)

Please be careful [if you use Nexus](https://github.com/open-archetypes/tycho-eclipse-plugin-archetype/issues/5)

For `kepler` update `MANIFEST.MF` as below in `.test` project (see [#3](https://github.com/open-archetypes/tycho-eclipse-plugin-archetype/issues/3))
`Require-Bundle: org.eclipse.jdt.junit4.runtime;bundle-version="1.1.0",
 org.junit;bundle-version="4.11.0"`

MIT License was chosen at <http://choosealicense.com/> 

<http://www.xiconeditor.com/> Online Icon Editor

Thanks to Bananeweizen for [help](http://stackoverflow.com/questions/18083936/eclipse-plugins-separate-editor-and-icons-assignment).

## Other 

Not used here, but you also may be interested in
 [A Maven Archetype for Hadoop Jobs](http://blog.mafr.de/2010/08/01/maven-archetype-hadoop/)
 
### Other links
 
 - <http://stackoverflow.com/questions/12402860/eclipse-ctrlspace-content-assist-hook>
 - <http://stackoverflow.com/questions/1103199/eclipse-plugin-editor>
 
 
