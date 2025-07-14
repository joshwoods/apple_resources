

- AppKit
- NSAlert
-  alertStyle 

Instance Property

# alertStyle

Indicates the alert’s severity level.

macOS

``` source
@MainActor
var alertStyle: NSAlert.Style { get set }
```

## Discussion

See the NSAlert.Style enumeration for the list of alert style constants.

## See Also

### Configuring Alerts

func layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

var accessoryView: NSView?

The alert’s accessory view.

var showsHelp: Bool

Specifies whether the alert has a help button.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

