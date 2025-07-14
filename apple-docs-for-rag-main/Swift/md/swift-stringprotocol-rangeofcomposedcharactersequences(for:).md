

- Swift
- StringProtocol
-  rangeOfComposedCharacterSequences(for:) 

Instance Method

# rangeOfComposedCharacterSequences(for:)

Returns the range in the string of the composed character sequences for a given range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfComposedCharacterSequences(for range: R) -> Range where R : RangeExpression, R.Bound == String.Index
```

