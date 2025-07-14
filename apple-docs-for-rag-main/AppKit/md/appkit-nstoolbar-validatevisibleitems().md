

- AppKit
- NSToolbar
-  validateVisibleItems() 

Instance Method

# validateVisibleItems()

Validates the toolbar’s visible items during a window update.

macOS

``` source
@MainActor
func validateVisibleItems()
```

## Discussion

Typically, you override this method and use it to customize the validation process. The default implementation calls the validate() method of each visible item in the toolbar, including items that have their autovalidates property set to false. If you override this method, call `super` at some point during your implementation.

The toolbar doesn’t validate its content for some events, including NSLeftMouseDragged, NSRightMouseDragged, NSOtherMouseDragged, NSMouseEntered, NSMouseExited, NSScrollWheel, NSCursorUpdate, NSKeyDown. In addition, the toolbar defers validation for NSKeyUp and NSFlagsChanged events until a pause of 0.85 seconds occurs or the window processes an event other than NSKeyUp or NSFlagsChanged. So a rapid sequence of key events doesn’t trigger any validation.

To trigger validation for all toolbars, call the app’s setWindowsNeedUpdate(_:) method with a value of true.

