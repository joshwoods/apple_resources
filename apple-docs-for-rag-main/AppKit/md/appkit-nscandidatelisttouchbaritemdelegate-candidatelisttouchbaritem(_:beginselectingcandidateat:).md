

- AppKit
- NSCandidateListTouchBarItemDelegate
-  candidateListTouchBarItem(\_:beginSelectingCandidateAt:) 

Instance Method

# candidateListTouchBarItem(\_:beginSelectingCandidateAt:)

Tells the delegate that the user has started touching one of the candidates in the candidate list item.

macOS 10.12.2+

``` source
@MainActor
optional func candidateListTouchBarItem(
    _ anItem: NSCandidateListTouchBarItem,
    beginSelectingCandidateAt index: Int
)
```

## Parameters 

`anItem`  

The candidate list bar item that the user is interacting with.

`index`  

The index of the candidate that the user is currently touching.

## See Also

### Handling selection changes

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, changeSelectionFromCandidateAt: Int, to: Int)

Tells the delegate that user has moved from touching one candidate in the candidate list item to another.

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, endSelectingCandidateAt: Int)

Tells the delegate that a user has stopped touching candidates in the candidate list item.

