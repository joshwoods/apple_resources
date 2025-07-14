

- AppKit
- NSTextView
-  orderFrontTablePanel(\_:) 

Instance Method

# orderFrontTablePanel(\_:)

Brings forward a panel allowing the user to manipulate text tables in the text view.

macOS

``` source
@MainActor
func orderFrontTablePanel(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message. May be `nil`.

## See Also

### Working with panels

var usesFontPanel: Bool

A Boolean value that controls whether the text views sharing the receiver’s layout manager use the Font panel and Font menu.

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

func orderFrontSubstitutionsPanel(Any?)

Brings forward a panel allowing the user to specify string substitutions in the text view.

