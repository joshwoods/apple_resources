

- AppKit
- NSViewController
-  presentAsSheet(\_:) 

Instance Method

# presentAsSheet(\_:)

Presents another view controller as a sheet.

macOS 10.10+

``` source
@MainActor
func presentAsSheet(_ viewController: NSViewController)
```

## Parameters 

`viewController`  

The other view controller to present as a sheet.

## Discussion

This method calls the present(_:animator:) method on `self` (the presenting view controller), and passes a sheet animator to that method.

The presented view controller is the delegate and the content view controller of its sheet.

To dismiss the sheet, call the dismiss(_:) method on `self` (the presenting view controller).

## See Also

### Presenting Another View Controller’s Content

func present(NSViewController, animator: any NSViewControllerPresentationAnimator)

Presents another view controller using a specified, custom animator for presentation and dismissal.

func dismiss(NSViewController)

Dismisses a presented view controller, using the same animator that presented it.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior)

Presents another view controller as a popover.

func present(NSViewController, asPopoverRelativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge, behavior: NSPopover.Behavior, hasFullSizeContent: Bool)

func presentAsModalWindow(NSViewController)

Presents another view controller as a modal window, also known as an alert.

func present(inWidget: NSViewController)Deprecated

