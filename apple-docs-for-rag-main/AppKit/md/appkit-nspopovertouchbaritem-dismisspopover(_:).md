

- AppKit
- NSPopoverTouchBarItem
-  dismissPopover(\_:) 

Instance Method

# dismissPopover(\_:)

Restores the previously visible main bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
func dismissPopover(_ sender: Any?)
```

## Discussion

This method has the same effect as the user tapping the optional close button.

## See Also

### Expanding and collapsing a popover

func showPopover(Any?)

Replaces the main bar with this item’s popover bar.

func makeStandardActivatePopoverGestureRecognizer() -> NSGestureRecognizer

Returns a gesture recognizer, configured to invoke the showPopover(_:) method.

