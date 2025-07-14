

- Foundation
- NSString
-  replacingOccurrences(of:with:options:range:) 

Instance Method

# replacingOccurrences(of:with:options:range:)

Returns a new string in which all occurrences of a target string in a specified range of the receiver are replaced by another given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacingOccurrences(
    of target: String,
    with replacement: String,
    options: NSString.CompareOptions = [],
    range searchRange: NSRange
) -> String
```

## Parameters 

`target`  

The string to replace.

`replacement`  

The string with which to replace `target`.

`options`  

A mask of options to use when comparing `target` with the receiver. Pass `0` to specify no options.

`searchRange`  

The range in the receiver in which to search for `target`.

## Return Value

A new string in which all occurrences of `target`, matched using `options`, in `searchRange` of the receiver are replaced by `replacement`.

## See Also

### Related Documentation

func replacingPercentEscapes(using: UInt) -> String?

Returns a new string made by replacing in the receiver all percent escapes with the matching characters as determined by a given encoding.

Deprecated

### Replacing Substrings

func replacingOccurrences(of: String, with: String) -> String

Returns a new string in which all occurrences of a target string in the receiver are replaced by another given string.

func replacingCharacters(in: NSRange, with: String) -> String

Returns a new string in which the characters in a specified range of the receiver are replaced by a given string.

