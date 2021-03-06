## 1.0.2

* Added accessor `notags`. It can be used with checklist for example. The default value is false.

 ```
 dialog = MRDialog.new()
 dialog.notags = true
 ```
* Added accessor `dialog_options`. It can be used to pass any valid dialog option. `man dialog` and look at the **OPTIONS** section. It is the caller's responsibily to specify correct options, no validation will be done. Example:

```
dialog = MRDialog.new()
dialog.dialog_options = "--no-tags"
```
This ia exactly same as `dialog.notags = true`

(Apr-16-2016 )

## 1.0.1

* Jeweler support for making the gem.

Implemented methods for: 

*  'buildlist' (--buildlist)
*  'editbox' (--editbox)
*  'form' (--form)
*  'gauge' (--gauge). Thanks to Mike Morgan.
*  'mixedform' (--mixedform)
*  'passwordform' (--mixedform)
*  'pause' (--pasue)
*  'prgbox' (--prgbox)
*  'progressbox' (--progressbox)
*  'progambox' (--programbox)
*  'treeview' (--treeview)

* Added accessors:
    "logger", "clear", "ok_label <label>", "insecure", "ascii_lines"
* Added methods to check dialog's exit code
    dialog_ok, dialog_cancel, dialog_help, dialog_extra,
    dialog_item_help, dialog_esc

Implemented examples for:

* buildlist
* calendar
* checklist
* editbox
* form
* fselect
* gauge
* infobox
* inputbox
* menu
* msgbox
* passwordbox
* pause
* prgbox
* progressbox
* programbox
* radiolist
* timebox
* treeview
* yesno

Note: The examples use Struct class, making the examples clean and 
easy to understand. 


# bug fixes:

* raise exception if 'dialog' program is not found.
* title in the option string was not quoted
* timebox syntax is different now.
etc..

-- muquit@muquit.com , Apr-05-2014, first cut

## 0.5.0

* original base code
