

- UIKit
- UITextDropProposal
-  dropProgressMode 

Instance Property

# dropProgressMode

A mode that specifies how the text view indicates progress to the user when loading dropped items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dropProgressMode: UITextDropProposal.ProgressMode { get set }
```

## Discussion

The default value is UITextDropProposal.ProgressMode.system.

## See Also

### Configuring a text drop proposal

var dropAction: UITextDropProposal.Action

A text drop action style that specifies how the text view receives dropped items.

enum Action

The text drop action styles for text views.

var dropPerformer: UITextDropProposal.Performer

The performer that is responsible for handling the drop operation.

enum Performer

The performers that are responsible for handling the drop operation.

enum ProgressMode

The text drop progress styles for user-visible progress indication.

var useFastSameViewOperations: Bool

A Boolean value that determines whether the text view can use fast inline dropping when the source and destination are in the same text view.

