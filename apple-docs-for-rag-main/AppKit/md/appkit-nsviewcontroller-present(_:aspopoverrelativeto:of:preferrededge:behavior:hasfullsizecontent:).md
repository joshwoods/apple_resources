

- AppKit
- NSViewController
-  present(\_:asPopoverRelativeTo:of:preferredEdge:behavior:hasFullSizeContent:) 

Instance Method

# present(\_:asPopoverRelativeTo:of:preferredEdge:behavior:hasFullSizeContent:)

macOS 14.0+

``` source
@MainActor
func present(
    _ viewController: NSViewController,
    asPopoverRelativeTo positioningRect: NSRect,
    of positioningView: NSView,
    preferredEdge: NSRectEdge,
    behavior: NSPopover.Behavior,
    hasFullSizeContent: Bool
)
```

## See Also

### Presenting Another View Controller’s Content

func present(NSViewController, animator: any NSViewControllerPresentationAnimator)

Presents another view controller using a specified, custom animator for presentation and dismissal.

func dismiss(NSViewController)

Dismisses a presented view controller, using the same animator that presented it.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior)

Presents another view controller as a popover.

func presentAsModalWindow(NSViewController)

Presents another view controller as a modal window, also known as an alert.

func presentAsSheet(NSViewController)

Presents another view controller as a sheet.

func present(inWidget: NSViewController)Deprecated

