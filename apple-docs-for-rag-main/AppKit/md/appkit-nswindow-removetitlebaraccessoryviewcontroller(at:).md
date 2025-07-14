

- AppKit
- NSWindow
-  removeTitlebarAccessoryViewController(at:) 

Instance Method

# removeTitlebarAccessoryViewController(at:)

Removes the view controller at the specified index from the window’s array of title bar accessory view controllers.

macOS 10.10+

``` source
@MainActor
func removeTitlebarAccessoryViewController(at index: Int)
```

## Parameters 

`index`  

The index in the array of title bar view controllers from which to remove the view controller.

## Discussion

You can also use removeFromParent() to remove a specific title bar accessory view controller.

## See Also

### Managing Title Bar Accessories

func addTitlebarAccessoryViewController(NSTitlebarAccessoryViewController)

Adds the specified title bar accessory view controller to the window.

func insertTitlebarAccessoryViewController(NSTitlebarAccessoryViewController, at: Int)

Inserts the view controller into the window’s array of title bar accessory view controllers at the specified index.

var titlebarAccessoryViewControllers: [NSTitlebarAccessoryViewController]

An array of title bar accessory view controllers that are currently added to the window.

