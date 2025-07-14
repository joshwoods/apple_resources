

- Swift
- StringProtocol
-  replacingOccurrences(of:with:options:range:) 

Instance Method

# replacingOccurrences(of:with:options:range:)

Returns a new string in which all occurrences of a target string in a specified range of the string are replaced by another given string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacingOccurrences(
    of target: Target,
    with replacement: Replacement,
    options: String.CompareOptions = [],
    range searchRange: Range? = nil
) -> String where Target : StringProtocol, Replacement : StringProtocol
```

