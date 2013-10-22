

# Nodeclipse Git Addon

Source at GitHub <https://github.com/Nodeclipse/org.nodeclipse.gitaddon>

## About

Associate *.git* files with TextEditor

![](with-git-addon.PNG)

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


## Ideas

check [issues](https://github.com/Nodeclipse/org.nodeclipse.gitaddon/issues)

## Tools

Help created with [GFM Viewer by Satyagraha](https://github.com/satyagraha/gfm_viewer)
 