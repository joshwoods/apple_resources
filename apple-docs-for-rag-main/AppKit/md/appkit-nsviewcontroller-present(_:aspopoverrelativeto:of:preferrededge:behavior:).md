

- AppKit
- NSViewController
-  present(\_:asPopoverRelativeTo:of:preferredEdge:behavior:) 

Instance Method

# present(\_:asPopoverRelativeTo:of:preferredEdge:behavior:)

Presents another view controller as a popover.

macOS 10.10+

``` source
@MainActor
func present(
    _ viewController: NSViewController,
    asPopoverRelativeTo positioningRect: NSRect,
    of positioningView: NSView,
    preferredEdge: NSRectEdge,
    behavior: NSPopover.Behavior
)
```

## Parameters 

`viewController`  

The other view controller to present as a popover.

`positioningRect`  

The content size of the popover.

`positioningView`  

The view relative to which the popover should be positioned. Must not be `nil`, or else the view controller raises an invalidArgumentException exception.

`preferredEdge`  

The edge of `positioningView` that the popover should prefer to be anchored to.

`behavior`  

The popover’s closing behavior. See the NSPopover.Behavior enumeration.

## Discussion

This method calls the present(_:animator:) method on `self` (the presenting view controller), and passes a popover animator to that method.

The presented view controller is the delegate and the content view controller of the popover. You can use NSPopoverDelegate methods to customize the popover.

To dismiss the popover, call the dismiss(_:) method on `self` (the presenting view controller).

## See Also

### Presenting Another View Controller’s Content

func present(NSViewController, animator: any NSViewControllerPresentationAnimator)

Presents another view controller using a specified, custom animator for presentation and dismissal.

func dismiss(NSViewController)

Dismisses a presented view controller, using the same animator that presented it.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior, hasFullSizeContent: Bool)

func presentAsModalWindow(NSViewController)

Presents another view controller as a modal window, also known as an alert.

func presentAsSheet(NSViewController)

Presents another view controller as a sheet.

func present(inWidget: NSViewController)Deprecated

