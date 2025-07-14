

- AppKit
- NSWindow
-  addTitlebarAccessoryViewController(\_:) 

Instance Method

# addTitlebarAccessoryViewController(\_:)

Adds the specified title bar accessory view controller to the window.

macOS 10.10+

``` source
@MainActor
func addTitlebarAccessoryViewController(_ childViewController: NSTitlebarAccessoryViewController)
```

## Parameters 

`childViewController`  

An instance of NSTitlebarAccessoryViewController containing the view to add, along with where to place it and how it should behave in full screen mode.

## See Also

### Managing Title Bar Accessories

func insertTitlebarAccessoryViewController(NSTitlebarAccessoryViewController, at: Int)

Inserts the view controller into the window’s array of title bar accessory view controllers at the specified index.

func removeTitlebarAccessoryViewController(at: Int)

Removes the view controller at the specified index from the window’s array of title bar accessory view controllers.

var titlebarAccessoryViewControllers: [NSTitlebarAccessoryViewController]

An array of title bar accessory view controllers that are currently added to the window.

