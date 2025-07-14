

- AppKit
- NSAlert
-  showsHelp 

Instance Property

# showsHelp

Specifies whether the alert has a help button.

macOS

``` source
@MainActor
var showsHelp: Bool { get set }
```

## Discussion

Set this property’s value to true to specify that the alert has a help button, or false to specify it does not.

When a user clicks an alert’s help button, the alert delegate (delegate) receives an alertShowHelp(_:) message. The delegate is responsible for displaying the help information related to this particular alert.

Clicking an alert’s help button can alternately cause the openHelpAnchor(_:inBook:) message to be sent to the app’s help manager with a `nil` book and the anchor specified by the helpAnchor property, if any of the following conditions are true:

- There is no alert delegate.

- The alert delegate does not implement alertShowHelp(_:).

- The alert delegate implements alertShowHelp(_:) but returns false. When this is the case, an exception is raised if no help anchor is set.

## See Also

### Configuring Alerts

func layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

var alertStyle: NSAlert.Style

Indicates the alert’s severity level.

var accessoryView: NSView?

The alert’s accessory view.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

