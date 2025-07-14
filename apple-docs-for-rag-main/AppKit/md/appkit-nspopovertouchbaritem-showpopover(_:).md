

- AppKit
- NSPopoverTouchBarItem
-  showPopover(\_:) 

Instance Method

# showPopover(\_:)

Replaces the main bar with this item’s popover bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
func showPopover(_ sender: Any?)
```

## Discussion

If this item is not visible, this method will have no effect.

## See Also

### Expanding and collapsing a popover

func dismissPopover(Any?)

Restores the previously visible main bar.

func makeStandardActivatePopoverGestureRecognizer() -> NSGestureRecognizer

Returns a gesture recognizer, configured to invoke the showPopover(_:) method.

