

- AppKit
- NSApplication
-  showHelp(\_:) 

Instance Method

# showHelp(\_:)

If your project is properly registered, and the necessary keys have been set in the property list, this method launches Help Viewer and displays the first page of your app’s help book.

macOS

``` source
@MainActor
func showHelp(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

For information on how to set up your project to take advantage of having Help Viewer display your help book, see Specifying the Comprehensive Help File.

## See Also

### Providing Help Information

func registerUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Register an object that provides help data to your app.

func searchString(String, inUserInterfaceItemString: String, range: NSRange, found: UnsafeMutablePointer&lt;NSRange>?) -> Bool

Searches for the string in the user interface.

func unregisterUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Unregister an object that provides help data to your app.

func activateContextHelpMode(Any?)

Places the receiver in context-sensitive help mode.

var helpMenu: NSMenu?

The help menu used by the app.

