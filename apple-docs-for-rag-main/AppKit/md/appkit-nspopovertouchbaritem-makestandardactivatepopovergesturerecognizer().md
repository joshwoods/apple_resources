

- AppKit
- NSPopoverTouchBarItem
-  makeStandardActivatePopoverGestureRecognizer() 

Instance Method

# makeStandardActivatePopoverGestureRecognizer()

Returns a gesture recognizer, configured to invoke the showPopover(_:) method.

macOS 10.12.2+

``` source
@MainActor
func makeStandardActivatePopoverGestureRecognizer() -> NSGestureRecognizer
```

## Discussion

Use this method to create a gesture recognizer that you then attach to a custom collapsedRepresentation view.

## See Also

### Expanding and collapsing a popover

func showPopover(Any?)

Replaces the main bar with this item’s popover bar.

func dismissPopover(Any?)

Restores the previously visible main bar.

