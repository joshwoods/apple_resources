

- AppKit
- NSApplication
-  helpMenu 

Instance Property

# helpMenu

The help menu used by the app.

macOS 10.6+

``` source
@MainActor
var helpMenu: NSMenu? { get set }
```

## Discussion

Use this property to specify your app’s Help menu. When this property contains a valid menu, the system installs its Spotlight-related menu items on that menu. When the value is `nil`, AppKit installs Spotlight menu items on the menu of its choosing. To suppress Spotlight help items altogether, specify a menu that doesn’t appear on the menu bar.

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

func activateContextHelpMode(Any?)

Places the receiver in context-sensitive help mode.

