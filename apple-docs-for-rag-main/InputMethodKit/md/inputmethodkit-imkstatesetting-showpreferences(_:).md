

- InputMethodKit
- IMKStateSetting
-  showPreferences(\_:) 

Instance Method

# showPreferences(\_:)

Displays a preferences window.

macOS 10.5+

``` source
func showPreferences(_ sender: Any!)
```

**Required**

## Parameters 

`sender`  

The object sending the message to show the preference window.

## Discussion

This method looks for a nib file that contains a window controller class and a preferences utility. If found, it displays the window. To use this method you must create a menu item in your input method menu whose action is `showPreferences:`. When a user selects that item, the Input Method Kit invokes your `showPreferences:` method. The default implementation looks for a nib file named `preferences.nib`. If found, it allocates a window controller class loads the nib file. You can provide a custom window controller class by naming the class in your input method `info.plist` file, providing a key-value pair. The key must be `InputMethodServerPreferencesWindowControllerClass` and the associated value must be the name of your custom class.

