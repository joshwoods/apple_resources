

- UIKit
- UITextDropProposal
-  dropAction 

Instance Property

# dropAction

A text drop action style that specifies how the text view receives dropped items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dropAction: UITextDropProposal.Action { get set }
```

## Discussion

The property’s default value is UITextDropProposal.Action.insert.

## See Also

### Configuring a text drop proposal

enum Action

The text drop action styles for text views.

var dropPerformer: UITextDropProposal.Performer

The performer that is responsible for handling the drop operation.

enum Performer

The performers that are responsible for handling the drop operation.

var dropProgressMode: UITextDropProposal.ProgressMode

A mode that specifies how the text view indicates progress to the user when loading dropped items.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

var useFastSameViewOperations: Bool

A Boolean value that determines whether the text view can use fast inline dropping when the source and destination are in the same text view.

