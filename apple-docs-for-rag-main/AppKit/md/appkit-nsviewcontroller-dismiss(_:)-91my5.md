

- AppKit
- NSViewController
-  dismiss(\_:) 

Instance Method

# dismiss(\_:)

Dismisses a presented view controller, using the same animator that presented it.

macOS 10.10+

``` source
@MainActor
func dismiss(_ viewController: NSViewController)
```

## Parameters 

`viewController`  

The presented view controller that you are dismissing.

## Discussion

In macOS, this is the universal way to dismiss a view controller, no matter how it was presented.

## See Also

### Presenting Another View Controller’s Content

func present(NSViewController, animator: any NSViewControllerPresentationAnimator)

Presents another view controller using a specified, custom animator for presentation and dismissal.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior)

Presents another view controller as a popover.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior, hasFullSizeContent: Bool)

func presentAsModalWindow(NSViewController)

Presents another view controller as a modal window, also known as an alert.

func presentAsSheet(NSViewController)

Presents another view controller as a sheet.

func present(inWidget: NSViewController)Deprecated

