

- AppKit
- NSCandidateListTouchBarItem
-  attributedStringForCandidate 

Instance Property

# attributedStringForCandidate

A block that converts a candidate object into an attributed string for display in the candidate list item.

macOS 10.12.2+

``` source
@MainActor
var attributedStringForCandidate: ((CandidateType, Int) -> NSAttributedString)? { get set }
```

## Discussion

This property is not required if the object type of your candidates is NSString, NSAttributedString, or NSTextCheckingResult. The default value of this property is `nil`.

If the attributed string you return does not specify font or foregroundColor then the candidate is displayed with the standard appearance font and color.

## See Also

### Populating the candidate list

func setCandidates([CandidateType], forSelectedRange: NSRange, in: String?)

Sets an array of candidate objects to be displayed in the candidate list bar item.

var candidates: [CandidateType]

The array of candidate objects previously set by setCandidates(_:forSelectedRange:in:).

var allowsTextInputContextCandidates: Bool

A Boolean value that specifies whether a candidate list item displays candidates from text input providers.

