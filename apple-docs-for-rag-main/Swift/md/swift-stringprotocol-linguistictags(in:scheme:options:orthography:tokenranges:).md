

- Swift
- StringProtocol
-  linguisticTags(in:scheme:options:orthography:tokenRanges:) 

Instance Method

# linguisticTags(in:scheme:options:orthography:tokenRanges:)

Returns an array of linguistic tags for the specified range and requested tags within the receiving string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func linguisticTags(
    in range: R,
    scheme tagScheme: T,
    options opts: NSLinguisticTagger.Options = [],
    orthography: NSOrthography? = nil,
    tokenRanges: UnsafeMutablePointer]>? = nil
) -> [String] where T : StringProtocol, R : RangeExpression, R.Bound == String.Index
```

