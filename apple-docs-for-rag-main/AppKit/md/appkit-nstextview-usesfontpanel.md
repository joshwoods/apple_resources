

- AppKit
- NSTextView
-  usesFontPanel 

Instance Property

# usesFontPanel

A Boolean value that controls whether the text views sharing the receiver’s layout manager use the Font panel and Font menu.

macOS

``` source
@MainActor
var usesFontPanel: Bool { get set }
```

## Discussion

true to make the text views sharing the receiver’s layout manager respond to messages from the Font panel and from the Font menu, and update the Font panel with the selection font whenever it changes, false to disallow character attribute changes.

## See Also

### Related Documentation

var rangeForUserCharacterAttributeChange: NSRange

The range of characters affected by an action method that changes character (not paragraph) attributes.

### Working with panels

var usesFindPanel: Bool

A Boolean value that indicates whether the receiver allows for a find panel.

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

