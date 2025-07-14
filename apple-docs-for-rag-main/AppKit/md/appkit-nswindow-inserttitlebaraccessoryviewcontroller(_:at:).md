

- AppKit
- NSWindow
-  insertTitlebarAccessoryViewController(\_:at:) 

Instance Method

# insertTitlebarAccessoryViewController(\_:at:)

Inserts the view controller into the window’s array of title bar accessory view controllers at the specified index.

macOS 10.10+

``` source
@MainActor
func insertTitlebarAccessoryViewController(
    _ childViewController: NSTitlebarAccessoryViewController,
    at index: Int
)
```

## Parameters 

`childViewController`  

The title bar accessory view controller to insert.

`index`  

The index at which to insert `childViewController`.

## See Also

### Managing Title Bar Accessories

func addTitlebarAccessoryViewController(NSTitlebarAccessoryViewController)

Adds the specified title bar accessory view controller to the window.

func removeTitlebarAccessoryViewController(at: Int)

Removes the view controller at the specified index from the window’s array of title bar accessory view controllers.

var titlebarAccessoryViewControllers: [NSTitlebarAccessoryViewController]

An array of title bar accessory view controllers that are currently added to the window.

