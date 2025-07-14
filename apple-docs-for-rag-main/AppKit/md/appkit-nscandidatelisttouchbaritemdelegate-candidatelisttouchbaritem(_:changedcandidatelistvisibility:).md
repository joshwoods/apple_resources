

- AppKit
- NSCandidateListTouchBarItemDelegate
-  candidateListTouchBarItem(\_:changedCandidateListVisibility:) 

Instance Method

# candidateListTouchBarItem(\_:changedCandidateListVisibility:)

Tells the delegate that the visibility of the candidate list has changed.

macOS 10.12.2+

``` source
@MainActor
optional func candidateListTouchBarItem(
    _ anItem: NSCandidateListTouchBarItem,
    changedCandidateListVisibility isVisible: Bool
)
```

## Parameters 

`anItem`  

The candidate list item whose candidate list’s visibility has changed.

`isVisible`  

A Boolean value that specifies whether or not the candidate list is visible. If true then the candidate list is visible, false otherwise.

