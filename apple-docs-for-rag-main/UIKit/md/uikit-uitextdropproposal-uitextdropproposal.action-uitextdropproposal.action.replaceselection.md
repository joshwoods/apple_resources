

- UIKit
- UITextDropProposal
- UITextDropProposal.Action
-  UITextDropProposal.Action.replaceSelection 

Case

# UITextDropProposal.Action.replaceSelection

A text drop action style specifying that if the target text view contains a selection, dropped text replaces it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case replaceSelection
```

## Discussion

If the text view does not contain a selection, dropped text is inserted at the provided location, without altering the surrounding text.

## See Also

### Text drop actions

case insert

A text drop action style specifying that text is inserted at the provided location, without altering the surrounding text.

case replaceAll

A text drop action style specifying that the dropped text replaces all text in the target text view.

