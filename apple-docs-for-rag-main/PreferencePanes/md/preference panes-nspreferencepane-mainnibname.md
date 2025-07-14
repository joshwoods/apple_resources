

- Preference Panes
- NSPreferencePane
-  mainNibName 

Instance Property

# mainNibName

The name of the preference pane’s nib file.

Mac Catalyst 14.0+macOS 10.1+

``` source
var mainNibName: String { get }
```

## Discussion

The name should not include the `.nib` extension.

The default implementation returns the value of the `NSMainNibFile` key in the bundle’s information property list. If the key does not exist, it returns a default value of `@”Main”`.

## See Also

### Getting the Bundle Information

var bundle: Bundle

The preference pane’s bundle.

var mainView: NSView

The main view of the preference pane.

