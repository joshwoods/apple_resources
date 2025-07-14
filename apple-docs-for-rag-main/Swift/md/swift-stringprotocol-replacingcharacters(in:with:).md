

- Swift
- StringProtocol
-  replacingCharacters(in:with:) 

Instance Method

# replacingCharacters(in:with:)

Returns a new string in which the characters in a specified range of the `String` are replaced by a given string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacingCharacters(
    in range: R,
    with replacement: T
) -> String where T : StringProtocol, R : RangeExpression, R.Bound == String.Index
```

