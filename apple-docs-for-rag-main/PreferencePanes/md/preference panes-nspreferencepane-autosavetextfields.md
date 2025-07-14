

- Preference Panes
- NSPreferencePane
-  autoSaveTextFields 

Instance Property

# autoSaveTextFields

A Boolean value that indicates whether text fields save their values before changing preference panes.

Mac Catalyst 14.0+macOS 10.1+

``` source
var autoSaveTextFields: Bool { get }
```

## Discussion

If this property is true, text fields are forced to give up their responder status before shouldUnselect is called on the preference pane. If it is false, the preference pane is responsible for forcing text fields to give up their responder status before saving them. The default value is true.

## See Also

### Handling keyboard focus

var firstKeyView: NSView?

The first view in the keyboard focus chain.

var initialKeyView: NSView?

The view that should have keyboard focus when the pane is selected.

var lastKeyView: NSView?

The last view in the keyboard focus chain.

