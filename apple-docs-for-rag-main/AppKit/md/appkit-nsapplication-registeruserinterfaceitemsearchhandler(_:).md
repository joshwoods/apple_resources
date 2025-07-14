

- AppKit
- NSApplication
-  registerUserInterfaceItemSearchHandler(\_:) 

Instance Method

# registerUserInterfaceItemSearchHandler(\_:)

Register an object that provides help data to your app.

macOS 10.6+

``` source
@MainActor
func registerUserInterfaceItemSearchHandler(_ handler: any NSUserInterfaceItemSearching)
```

## Parameters 

`handler`  

The class instance that conforms to `NSUserInterfaceItemSearching` and provides help content.

## Discussion

You can register as many search handlers as you like. If you register the same instance more than once the subsequent registrations are ignored.

## See Also

### Providing Help Information

func searchString(String, inUserInterfaceItemString: String, range: NSRange, found: UnsafeMutablePointer&lt;NSRange>?) -> Bool

Searches for the string in the user interface.

func unregisterUserInterfaceItemSearchHandler(any NSUserInterfaceItemSearching)

Unregister an object that provides help data to your app.

func showHelp(Any?)

If your project is properly registered, and the necessary keys have been set in the property list, this method launches Help Viewer and displays the first page of your app’s help book.

func activateContextHelpMode(Any?)

Places the receiver in context-sensitive help mode.

var helpMenu: NSMenu?

The help menu used by the app.

