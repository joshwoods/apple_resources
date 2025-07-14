

- AppKit
- NSTitlebarAccessoryViewController
-  viewWillAppear() 

Instance Method

# viewWillAppear()

Called after the title bar accessory view controller’s view has been loaded into memory is about to be added to the view hierarchy in the window.

macOS 10.10+

``` source
@MainActor
func viewWillAppear()
```

## Discussion

This method is called when the accessory view is about to be added to the window’s view hierarchy or the window is about to become visible, such as coming to the front or becoming unhidden. If you override this method, you must call `super` in your implementation.

## See Also

### Responding to View Events

func viewDidAppear()

Called when the title bar accessory view controller’s view is fully transitioned onto the screen.

func viewDidDisappear()

Called after the title bar accessory view controller’s view is removed from the window’s view hierarchy.

