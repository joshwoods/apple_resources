

- UIKit
- UITextDropProposal
-  dropPerformer 

Instance Property

# dropPerformer

The performer that is responsible for handling the drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dropPerformer: UITextDropProposal.Performer { get set }
```

## Discussion

The performer provides a preview for the drop activity, loads the data from the item providers, and inserts the data into the text view. It can be the UITextDropProposal.Performer.view performer (default) or the UITextDropProposal.Performer.delegate performer.

## See Also

### Configuring a text drop proposal

var dropAction: UITextDropProposal.Action

A text drop action style that specifies how the text view receives dropped items.

enum Action

The text drop action styles for text views.

enum Performer

The performers that are responsible for handling the drop operation.

var dropProgressMode: UITextDropProposal.ProgressMode

A mode that specifies how the text view indicates progress to the user when loading dropped items.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

var useFastSameViewOperations: Bool

A Boolean value that determines whether the text view can use fast inline dropping when the source and destination are in the same text view.

