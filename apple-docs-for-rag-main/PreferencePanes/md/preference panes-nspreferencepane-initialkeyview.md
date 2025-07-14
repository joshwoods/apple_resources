

- Preference Panes
- NSPreferencePane
-  initialKeyView 

Instance Property

# initialKeyView

The view that should have keyboard focus when the pane is selected.

Mac Catalyst 14.0+macOS 10.1+

``` source
var initialKeyView: NSView? { get set }
```

## Discussion

The initial view can be set in the nib file by connecting a view to the receiver’s `_initialKeyView` outlet.

## See Also

### Handling keyboard focus

var firstKeyView: NSView?

The first view in the keyboard focus chain.

var lastKeyView: NSView?

The last view in the keyboard focus chain.

var autoSaveTextFields: Bool

A Boolean value that indicates whether text fields save their values before changing preference panes.

