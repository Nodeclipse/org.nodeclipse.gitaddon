
## About

Associate *.git* files with TextEditor

![](with-git-addon.PNG)

Builded againt Indigo and tested in Kepler.

## Install from sources

`mvn package`  
`npm install http-server -g`
`http-server gitaddon.site\target\repository`
start http://localhost:8080/
// navigate `http://localhost:8080/` in browser to check
Help->Install New Software, enter http://localhost:8080/ in Work With

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

## Other 

Not used here, but you also may be interested in
 [A Maven Archetype for Hadoop Jobs](http://blog.mafr.de/2010/08/01/maven-archetype-hadoop/)
