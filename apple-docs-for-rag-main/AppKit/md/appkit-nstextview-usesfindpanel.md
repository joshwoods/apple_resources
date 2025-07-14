

- AppKit
- NSTextView
-  usesFindPanel 

Instance Property

# usesFindPanel

A Boolean value that indicates whether the receiver allows for a find panel.

macOS

``` source
@MainActor
var usesFindPanel: Bool { get set }
```

## Discussion

true to allow the use of a find panel, false otherwise. A text view can use either a find panel or a find bar. If usesFindPanel is set to true, usesFindBar is set to false and vice versa.

## See Also

### Related Documentation

var usesFindBar: Bool

A Boolean value that indicates whether to use the find bar for this text view.

### Working with panels

var usesFontPanel: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager use the Font panel and Font menu.

func performFindPanelAction(Any?)

Performs a find panel action specified by the sender’s tag.

func orderFrontLinkPanel(Any?)

Brings forward a panel allowing the user to manipulate links in the text view.

func orderFrontListPanel(Any?)

Brings forward a panel allowing the user to manipulate text lists in the text view.

func orderFrontSpacingPanel(Any?)

Brings forward a panel allowing the user to manipulate text line heights, interline spacing, and paragraph spacing, in the text view.

func orderFrontTablePanel(Any?)

Brings forward a panel allowing the user to manipulate text tables in the text view.

func orderFrontSubstitutionsPanel(Any?)

Brings forward a panel allowing the user to specify string substitutions in the text view.

