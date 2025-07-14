

- AppKit
- NSCandidateListTouchBarItem
-  setCandidates(\_:forSelectedRange:in:) 

Instance Method

# setCandidates(\_:forSelectedRange:in:)

Sets an array of candidate objects to be displayed in the candidate list bar item.

macOS 10.12.2+

``` source
@MainActor
func setCandidates(
    _ candidates: [CandidateType],
    forSelectedRange selectedRange: NSRange,
    in originalString: String?
)
```

## Parameters 

`candidates`  

The array of candidates you wish to display in the candidate list item.

`selectedRange`  

A range (NSRange) within the string that the candidates represent.

`originalString`  

The original string from which the candidate list was derived.

## Discussion

The item uses the block in the attributedStringForCandidate property to convert each candidate in the array into an attributed string. If the value of the attributedStringForCandidate property is `nil` then NSCandidateListTouchBarItem can format candidates of type NSString, NSAttributedString, and NSTextCheckingResult.

## See Also

### Populating the candidate list

var candidates: [CandidateType]

The array of candidate objects previously set by setCandidates(_:forSelectedRange:in:).

var attributedStringForCandidate: ((CandidateType, Int) -> NSAttributedString)?

A block that converts a candidate object into an attributed string for display in the candidate list item.

var allowsTextInputContextCandidates: Bool

A Boolean value that specifies whether a candidate list item displays candidates from text input providers.

