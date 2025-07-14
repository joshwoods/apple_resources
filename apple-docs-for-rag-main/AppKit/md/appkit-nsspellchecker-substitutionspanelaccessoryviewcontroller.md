

- AppKit
- NSSpellChecker
-  substitutionsPanelAccessoryViewController 

Instance Property

# substitutionsPanelAccessoryViewController

Sets the substitutions panel’s accessory view.

macOS 10.6+

``` source
var substitutionsPanelAccessoryViewController: NSViewController? { get set }
```

## Parameters 

`accessoryController`  

The accessory view controller or `nil` if there is none.

## Discussion

The accessory view controller can accommodate any custom view you want to display with the substitutions panel. The accessory view controller’s view is displayed below the substitutions list and the panel automatically resizes to accommodate the accessory view.

This method posts a notification named didResizeNotification with the substitutions panel object to the default notification center.

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

var accessoryView: NSView?

Makes a view an accessory of the Spelling panel by making it a subview of the panel’s content view.

