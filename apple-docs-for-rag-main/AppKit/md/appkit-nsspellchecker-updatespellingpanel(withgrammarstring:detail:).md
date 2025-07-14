

- AppKit
- NSSpellChecker
-  updateSpellingPanel(withGrammarString:detail:) 

Instance Method

# updateSpellingPanel(withGrammarString:detail:)

Specifies a grammar-analysis detail to highlight in the Spelling panel.

macOS 10.5+

``` source
func updateSpellingPanel(
    withGrammarString string: String,
    detail: [String : Any]
)
```

## Parameters 

`string`  

Problematic grammatical unit identified by checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:).

`detail`  

One of the grammar-analysis details provided by checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:).

## See Also

### Managing Panels

var spellingPanel: NSPanel

Returns the spell checker’s panel.

var substitutionsPanel: NSPanel

Returns the substitutions panel.

func updatePanels()

Updates the available panels to account for user changes.

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

