

- AppKit
- NSSpellChecker
-  substitutionsPanel 

Instance Property

# substitutionsPanel

Returns the substitutions panel.

macOS 10.6+

``` source
var substitutionsPanel: NSPanel { get }
```

## Return Value

The substitutions checking panel.

## See Also

### Managing Panels

var spellingPanel: NSPanel

Returns the spell checker’s panel.

func updateSpellingPanel(withGrammarString: String, detail: [String : Any])

Specifies a grammar-analysis detail to highlight in the Spelling panel.

func updatePanels()

Updates the available panels to account for user changes.

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

