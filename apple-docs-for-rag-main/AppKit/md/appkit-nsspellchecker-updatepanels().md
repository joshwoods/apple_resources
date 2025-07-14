

- AppKit
- NSSpellChecker
-  updatePanels() 

Instance Method

# updatePanels()

Updates the available panels to account for user changes.

macOS 10.6+

``` source
func updatePanels()
```

## Discussion

This method should be called when a client changes some relevant setting, such as what kind of spelling, grammar checking, or substitutions it uses.

## See Also

### Managing Panels

var spellingPanel: NSPanel

Returns the spell checker’s panel.

var substitutionsPanel: NSPanel

Returns the substitutions panel.

func updateSpellingPanel(withGrammarString: String, detail: [String : Any])

Specifies a grammar-analysis detail to highlight in the Spelling panel.

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

