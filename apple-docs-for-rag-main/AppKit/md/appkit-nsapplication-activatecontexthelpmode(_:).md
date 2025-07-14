

- AppKit
- NSApplication
-  activateContextHelpMode(\_:) 

Instance Method

# activateContextHelpMode(\_:)

Places the receiver in context-sensitive help mode.

macOS

``` source
@MainActor
func activateContextHelpMode(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

In this mode, the cursor becomes a question mark, and help appears for any user interface item the user clicks.

Most apps don’t use this method. Instead, apps enter context-sensitive mode when the user presses the Help key. Apps exit context-sensitive help mode upon the first event after a help window is displayed.

## See Also

### Providing Help Information

func registerUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Register an object that provides help data to your app.

func searchString(String, inUserInterfaceItemString: String, range: NSRange, found: UnsafeMutablePointer&lt;NSRange>?) -> Bool

Searches for the string in the user interface.

func unregisterUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Unregister an object that provides help data to your app.

func showHelp(Any?)

If your project is properly registered, and the necessary keys have been set in the property list, this method launches Help Viewer and displays the first page of your app’s help book.

var helpMenu: NSMenu?

The help menu used by the app.

