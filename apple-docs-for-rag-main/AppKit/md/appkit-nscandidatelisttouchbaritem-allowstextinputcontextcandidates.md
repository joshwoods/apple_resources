

- AppKit
- NSCandidateListTouchBarItem
-  allowsTextInputContextCandidates 

Instance Property

# allowsTextInputContextCandidates

A Boolean value that specifies whether a candidate list item displays candidates from text input providers.

macOS 10.12.2+

``` source
@MainActor
var allowsTextInputContextCandidates: Bool { get set }
```

## Discussion

When true, the candidate list item shows candidates from the text input client provided in the client property, before those in the candidates property.

The default value of this property is true.

## See Also

### Populating the candidate list

func setCandidates([CandidateType], forSelectedRange: NSRange, in: String?)

Sets an array of candidate objects to be displayed in the candidate list bar item.

var candidates: [CandidateType]

The array of candidate objects previously set by setCandidates(_:forSelectedRange:in:).

var attributedStringForCandidate: ((CandidateType, Int) -> NSAttributedString)?

A block that converts a candidate object into an attributed string for display in the candidate list item.

