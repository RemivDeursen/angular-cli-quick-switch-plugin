# angular-cli-quick-switch-plugin

IntelliJ Plugin for switching between Angular CLI component files efficiently (ts -> html -> css -> scss) by using just a shortcut.

For example let's say we have a structure like this

    foo/
        foo.component.html
        foo.md
        foo.component.scss
        foo.component.ts

and we have selected the file **foo.component.ts**. By pressing the assigned shortcut repeatedly, the IDE will cycle
the files (i.e. closing the current tab and replacing it by the next one in the cycle) as follows:

    foo.component.ts -> foo.component.html -> foo.component.scss -> foo.component.ts

Whilst the default shortcut is registered with **Alt + S**, you can of course easily adjust this in the keymap settings by replacing it for **QuickSwitch**.

Note:
Due to the nature of this plugin, it will of course also work with other projects, that have not been generated by Angular CLI - or are
not even Angular projects at all - as long as your project structure follows similar patterns (namely all files of a component
have the exact same path, except for their file extension - and you are cycling between ts, html, css or scss files)