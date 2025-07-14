

- AppKit
- NSViewController
-  present(\_:animator:) 

Instance Method

# present(\_:animator:)

Presents another view controller using a specified, custom animator for presentation and dismissal.

macOS 10.10+

``` source
@MainActor
func present(
    _ viewController: NSViewController,
    animator: any NSViewControllerPresentationAnimator
)
```

## Parameters 

`viewController`  

The other view controller to present from the view controller.

Note

The view controller you provide in this parameter must not already be visible elsewhere, or else this method raises an exception.

The view in the presented view controller must have a window, or else this method raises an exception.

`animator`  

The animation delegate to employ for presentation and dismissal of the other view controller. The animator that you specify is retained until the dismiss(_:) method is called and the dismissal animation completes.

Note

This parameter’s value must not be `nil`, or else this method raises an exception.

## Discussion

Do not call this method unless you want to use a custom animator. To use one of the standard animators to present another view controller, instead call one of the dedicated presentation methods:

- present(_:asPopoverRelativeTo:of:preferredEdge:behavior:)

- presentAsModalWindow(_:)

- presentAsSheet(_:)

Each of these methods calls this method in turn. User interaction is blocked during presentation and dismissal.

## See Also

### Presenting Another View Controller’s Content

func dismiss(NSViewController)

Dismisses a presented view controller, using the same animator that presented it.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior)

Presents another view controller as a popover.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior, hasFullSizeContent: Bool)

func presentAsModalWindow(NSViewController)

Presents another view controller as a modal window, also known as an alert.

func presentAsSheet(NSViewController)

Presents another view controller as a sheet.

func present(inWidget: NSViewController)Deprecated

