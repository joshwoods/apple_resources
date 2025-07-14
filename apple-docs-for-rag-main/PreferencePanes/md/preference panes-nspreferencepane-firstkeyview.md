

- Preference Panes
- NSPreferencePane
-  firstKeyView 

Instance Property

# firstKeyView

The first view in the keyboard focus chain.

Mac Catalyst 14.0+macOS 10.1+

``` source
var firstKeyView: NSView? { get set }
```

## Discussion

The first key view can be set in the nib file by connecting a view to the receiver’s `_firstKeyView` outlet.

## See Also

### Handling keyboard focus

var initialKeyView: NSView?

The view that should have keyboard focus when the pane is selected.

var lastKeyView: NSView?

The last view in the keyboard focus chain.

var autoSaveTextFields: Bool

A Boolean value that indicates whether text fields save their values before changing preference panes.

