

- Swift
- StringProtocol
-  enumerateLinguisticTags(in:scheme:options:orthography:invoking:) 

Instance Method

# enumerateLinguisticTags(in:scheme:options:orthography:invoking:)

Performs linguistic analysis on the specified string by enumerating the specific range of the string, providing the Block with the located tags.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateLinguisticTags(
    in range: R,
    scheme tagScheme: T,
    options opts: NSLinguisticTagger.Options = [],
    orthography: NSOrthography? = nil,
    invoking body: (String, Range, Range, inout Bool) -> Void
) where T : StringProtocol, R : RangeExpression, R.Bound == String.Index
```

