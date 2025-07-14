

- AppKit
- NSSpellChecker
-  spellingPanel 

Instance Property

# spellingPanel

Returns the spell checker’s panel.

macOS

``` source
var spellingPanel: NSPanel { get }
```

## Return Value

The spell checking panel.

## See Also

### Managing Panels

var substitutionsPanel: NSPanel

Returns the substitutions panel.

func updateSpellingPanel(withGrammarString: String, detail: [String : Any])

Specifies a grammar-analysis detail to highlight in the Spelling panel.

func updatePanels()

Updates the available panels to account for user changes.

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

