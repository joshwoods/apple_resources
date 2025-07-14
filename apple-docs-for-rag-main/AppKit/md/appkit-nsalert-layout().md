

- AppKit
- NSAlert
-  layout() 

Instance Method

# layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

macOS 10.5+

``` source
@MainActor
func layout()
```

## Discussion

You need to call this method only when you need to customize the alert’s layout. Call this method after all the alert’s attributes have been customized, including the suppression checkbox and the accessory layout. After the method returns, you can make the necessary layout changes; for example, adjusting the frame of the accessory view.

Note

The standard alert layout is subject to change in future system software versions. Therefore, if you rely on custom alert layout, you should make sure your layouts work as expected in future releases of macOS.

## See Also

### Configuring Alerts

var alertStyle: NSAlert.Style

Indicates the alert’s severity level.

var accessoryView: NSView?

The alert’s accessory view.

var showsHelp: Bool

Specifies whether the alert has a help button.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

