

- Foundation
- NSString
-  replacingOccurrences(of:with:) 

Instance Method

# replacingOccurrences(of:with:)

Returns a new string in which all occurrences of a target string in the receiver are replaced by another given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacingOccurrences(
    of target: String,
    with replacement: String
) -> String
```

## Parameters 

`target`  

The string to replace.

`replacement`  

The string with which to replace `target`.

## Return Value

A new string in which all occurrences of `target` in the receiver are replaced by `replacement`.

## Discussion

Invokes replacingOccurrences(of:with:options:range:)with `0` options and range of the whole string.

## See Also

### Related Documentation

func replacingPercentEscapes(using: UInt) -> String?

Returns a new string made by replacing in the receiver all percent escapes with the matching characters as determined by a given encoding.

Deprecated

### Replacing Substrings

func replacingOccurrences(of: String, with: String, options: NSString.CompareOptions, range: NSRange) -> String

Returns a new string in which all occurrences of a target string in a specified range of the receiver are replaced by another given string.

func replacingCharacters(in: NSRange, with: String) -> String

Returns a new string in which the characters in a specified range of the receiver are replaced by a given string.

