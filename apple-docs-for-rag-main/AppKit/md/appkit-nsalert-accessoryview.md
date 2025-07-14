

- AppKit
- NSAlert
-  accessoryView 

Instance Property

# accessoryView

The alert’s accessory view.

macOS 10.5+

``` source
@MainActor
var accessoryView: NSView? { get set }
```

## Discussion

The NSAlert class places the accessory view between the informative text or suppression checkbox (if present) and the response buttons. Before you change the location of the accessory view, first call the layout() method.

alertStyle shows an example of adding an accessory view to an alert. buttons shows the alert generated.

Listing 1. Adding an accessory view to an alert

```
NSTextView *accessory = [[NSTextView alloc] initWithFrame:NSMakeRect(0,0,200,15)];
NSFont *font = [NSFont systemFontOfSize:[NSFont systemFontSize]];
NSDictionary *textAttributes = [NSDictionary dictionaryWithObject:font forKey:NSFontAttributeName];
[accessory insertText:[[NSAttributedString alloc] initWithString:@"Text in accessory view."
                                                      attributes:textAttributes]];
[accessory setEditable:NO];
[accessory setDrawsBackground:NO];

NSAlert *alert = [[NSAlert alloc] init];
alert.messageText = @"Message text.";
[alert setInformativeText:@"Informative text."];
alert.accessoryView = accessory;
[alert runModal];
[alert release];
```

## See Also

### Configuring Alerts

func layout()

Specifies that the alert must do immediate layout instead of lazily just before display.

var alertStyle: NSAlert.Style

Indicates the alert’s severity level.

var showsHelp: Bool

Specifies whether the alert has a help button.

var helpAnchor: NSHelpManager.AnchorName?

The alert’s HTML help anchor.

var delegate: (any NSAlertDelegate)?

The alert’s delegate.

