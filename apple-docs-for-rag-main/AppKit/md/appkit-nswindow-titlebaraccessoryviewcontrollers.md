

- AppKit
- NSWindow
-  titlebarAccessoryViewControllers 

Instance Property

# titlebarAccessoryViewControllers

An array of title bar accessory view controllers that are currently added to the window.

macOS 10.10+

``` source
@MainActor
var titlebarAccessoryViewControllers: [NSTitlebarAccessoryViewController] { get set }
```

## See Also

### Managing Title Bar Accessories

func addTitlebarAccessoryViewController(NSTitlebarAccessoryViewController)

Adds the specified title bar accessory view controller to the window.

func insertTitlebarAccessoryViewController(NSTitlebarAccessoryViewController, at: Int)

Inserts the view controller into the window’s array of title bar accessory view controllers at the specified index.

func removeTitlebarAccessoryViewController(at: Int)

Removes the view controller at the specified index from the window’s array of title bar accessory view controllers.

