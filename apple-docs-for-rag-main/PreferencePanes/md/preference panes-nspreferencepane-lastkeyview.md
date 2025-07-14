

- Preference Panes
- NSPreferencePane
-  lastKeyView 

Instance Property

# lastKeyView

The last view in the keyboard focus chain.

Mac Catalyst 14.0+macOS 10.1+

``` source
var lastKeyView: NSView? { get set }
```

## Discussion

The last view can be set in the nib file by connecting a view to the receiver’s `_lastKeyView` outlet.

## See Also

### Handling keyboard focus

var firstKeyView: NSView?

The first view in the keyboard focus chain.

var initialKeyView: NSView?

The view that should have keyboard focus when the pane is selected.

var autoSaveTextFields: Bool

A Boolean value that indicates whether text fields save their values before changing preference panes.

