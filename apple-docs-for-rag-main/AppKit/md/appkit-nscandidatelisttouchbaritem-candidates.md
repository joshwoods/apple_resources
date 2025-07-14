

- AppKit
- NSCandidateListTouchBarItem
-  candidates 

Instance Property

# candidates

The array of candidate objects previously set by setCandidates(_:forSelectedRange:in:).

macOS 10.12.2+

``` source
@MainActor
var candidates: [CandidateType] { get }
```

## See Also

### Populating the candidate list

func setCandidates([CandidateType], forSelectedRange: NSRange, in: String?)

Sets an array of candidate objects to be displayed in the candidate list bar item.

var attributedStringForCandidate: ((CandidateType, Int) -> NSAttributedString)?

A block that converts a candidate object into an attributed string for display in the candidate list item.

var allowsTextInputContextCandidates: Bool

A Boolean value that specifies whether a candidate list item displays candidates from text input providers.

