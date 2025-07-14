

- UIKit
- UITextDropProposal
- UITextDropProposal.Action
-  UITextDropProposal.Action.insert 

Case

# UITextDropProposal.Action.insert

A text drop action style specifying that text is inserted at the provided location, without altering the surrounding text.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case insert
```

## Discussion

The action ignores any selection present in the target text view.

## See Also

### Text drop actions

case replaceAll

A text drop action style specifying that the dropped text replaces all text in the target text view.

case replaceSelection

A text drop action style specifying that if the target text view contains a selection, dropped text replaces it.

