# NetBeans Settings For Laravel 4 Projects 
### By Mike Jackson | mrjxn @ MrJxN.com | github.com/mrjxn
## Description

NetBeans Settings for Laravel 4 Projects

A collection of NetBeans 7.4 settings .xml files to assist in Laravel 4 project development. 
NetBeans does not allow for independent export of each settings tab's sub-categories (e.g. Settings->Editor->Formatting->Language->PHP) so I am providing the following files separately to prevent overwriting unrelated settings, such as your formatting settings for other languages.  

* #### PHP Formatting

        <userdir> /config/Editors/text/x-php5/Preferences/org-netbeans-modules-editor-settings-CustomPreferences.xml
    * Please see NetBeans bug report here regarding the unsupported '<?php namespace ...' formatting: https://netbeans.org/bugzilla/show_bug.cgi?id=235710

* #### PHP Code Templates - WIP

        <userdir> /config/Editors/text/x-php5/CodeTemplates/org-netbeans-modules-editor-settings-CustomCodeTemplates.xml
    * Usage: After import, just type the shortcut then press tab (or alternative, if so customized) to begin the step-by-step autocomplete process (pressing enter after each argument) 
    * Current Templates:
        * lrte - Route::{verb}({arg},function({arg}) { return {arg}; });

## Installation

Unzip each file to your \<userdir> location - by default, located at:

* Windows: 
    
        C:\Users\<username>\AppData\Roaming\<nb-version>

* OSX:  

        /Users/<username>/Library/Application Support/<nb-version>

* Linux: 

        /home/<username>/.netbeans/<nb-version>

Ensure you unzip using the included directory structure to place the files in the correct place. 
NetBeans uses non-unique file names for it's settings .xml files, differentiated only by directory location.

## Notes

I recommend creating multiple versions of your userdir when making settings changes, 
especially when using dev/nightly versions of NetBeans. This ensures you can always easily revert to previous versions if you get lost.  
Add the --userdir \<userdir> argument when starting NetBeans to load the new userdir location.  For example, in Windows:

"C:\Program Files\NetBeans Dev 201309090001\bin\netbeans64.exe" --userdir D:\Dev-Web\Workspace\NetBeans\ \<myuserdir>

NetBeans settings files only contain entries for those items that differ from the defaults - for this reason, if you happen to inspect the files, you will notice only a fraction of the available settings are present.