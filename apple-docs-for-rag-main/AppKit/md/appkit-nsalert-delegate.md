

- AppKit
- NSAlert
-  delegate 

Instance Property

# delegate

The alert’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSAlertDelegate)? { get set }
```

## Discussion

To set a delegate for the alert, provide an object conforming to the NSAlertDelegateprotocol to this property. To remove the delegate, set this property’s value to `nil`.

## See Also

### Configuring Alerts

func layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

var alertStyle: NSAlert.Style

Indicates the alert’s severity level.

var accessoryView: NSView?

The alert’s accessory view.

var showsHelp: Bool

Specifies whether the alert has a help button.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

