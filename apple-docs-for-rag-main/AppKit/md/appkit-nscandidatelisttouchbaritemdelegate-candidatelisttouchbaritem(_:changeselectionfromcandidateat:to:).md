

- AppKit
- NSCandidateListTouchBarItemDelegate
-  candidateListTouchBarItem(\_:changeSelectionFromCandidateAt:to:) 

Instance Method

# candidateListTouchBarItem(\_:changeSelectionFromCandidateAt:to:)

Tells the delegate that user has moved from touching one candidate in the candidate list item to another.

macOS 10.12.2+

``` source
@MainActor
optional func candidateListTouchBarItem(
    _ anItem: NSCandidateListTouchBarItem,
    changeSelectionFromCandidateAt previousIndex: Int,
    to index: Int
)
```

## Parameters 

`anItem`  

The candidate list item that the user is interacting with.

`previousIndex`  

The index of the candidate that the user was previously touching.

`index`  

The index of the candidate that the user is currently touching.

## See Also

### Handling selection changes

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, beginSelectingCandidateAt: Int)

Tells the delegate that the user has started touching one of the candidates in the candidate list item.

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, endSelectingCandidateAt: Int)

Tells the delegate that a user has stopped touching candidates in the candidate list item.

