

- AppKit
- NSAlert
-  helpAnchor 

Instance Property

# helpAnchor

The alert’s HTML help anchor.

macOS

``` source
@MainActor
var helpAnchor: NSHelpManager.AnchorName? { get set }
```

## Discussion

To provide a help anchor for the alert, set this property to the appropriate string value. To remove the help anchor, set this property’s value to `nil`.

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

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

