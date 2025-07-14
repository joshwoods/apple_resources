

- AppKit
- NSCandidateListTouchBarItemDelegate
-  candidateListTouchBarItem(\_:endSelectingCandidateAt:) 

Instance Method

# candidateListTouchBarItem(\_:endSelectingCandidateAt:)

Tells the delegate that a user has stopped touching candidates in the candidate list item.

macOS 10.12.2+

``` source
@MainActor
optional func candidateListTouchBarItem(
    _ anItem: NSCandidateListTouchBarItem,
    endSelectingCandidateAt index: Int
)
```

## Parameters 

`anItem`  

The candidate list item that the user is interacting with.

`index`  

The index of the candidate that the user was touching when they lifted their finger.

## Discussion

If `index` is equal to `NSNotFound` then the user didn’t select a candidate.

## See Also

### Handling selection changes

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, beginSelectingCandidateAt: Int)

Tells the delegate that the user has started touching one of the candidates in the candidate list item.

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, changeSelectionFromCandidateAt: Int, to: Int)

Tells the delegate that user has moved from touching one candidate in the candidate list item to another.

