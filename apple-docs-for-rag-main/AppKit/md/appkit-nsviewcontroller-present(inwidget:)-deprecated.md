

- AppKit
- NSViewController
-  present(inWidget:) Deprecated

Instance Method

# present(inWidget:)

macOS 10.10–11.0Deprecated

``` source
@MainActor
func present(inWidget viewController: NSViewController)
```

Deprecated

Use WidgetKit instead. Today View extensions have been deprecated.

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

func presentAsSheet(NSViewController)

Presents another view controller as a sheet.

