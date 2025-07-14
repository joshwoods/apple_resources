

- AppKit
- NSSpellChecker
-  accessoryView 

Instance Property

# accessoryView

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

macOS

``` source
var accessoryView: NSView? { get set }
```

## Parameters 

`aView`  

The accessory view displayed in the receiver.

## Discussion

The accessory view can be any custom view you want to display with the spelling panel. The accessory view is displayed below the spelling checker and the panel automatically resizes to accommodate the accessory view.

This method posts a notification named didResizeNotification with the Spelling panel object to the default notification center.

## See Also

### Managing Panels

var spellingPanel: NSPanel

Returns the spell checker’s panel.

var substitutionsPanel: NSPanel

Returns the substitutions panel.

func updateSpellingPanel(withGrammarString: String, detail: [String : Any])

Specifies a grammar-analysis detail to highlight in the Spelling panel.

func updatePanels()

Updates the available panels to account for user changes.

var substitutionsPanelAccessoryViewController: NSViewController?

Sets the substitutions panel’s accessory view.

