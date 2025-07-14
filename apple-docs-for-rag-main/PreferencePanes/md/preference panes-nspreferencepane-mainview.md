

- Preference Panes
- NSPreferencePane
-  mainView 

Instance Property

# mainView

The main view of the preference pane.

Mac Catalyst 14.0+macOS 10.1+

``` source
var mainView: NSView { get set }
```

## Discussion

Subclasses should not need to override this unless they override loadMainView() or assignMainView().

## See Also

### Getting the Bundle Information

var bundle: Bundle

The preference pane’s bundle.

var mainNibName: String

The name of the preference pane’s nib file.

