

- Foundation
- NSRegularExpression
-  rangeOfFirstMatch(in:options:range:) 

Instance Method

# rangeOfFirstMatch(in:options:range:)

Returns the range of the first match of the regular expression within the specified range of the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rangeOfFirstMatch(
    in string: String,
    options: NSRegularExpression.MatchingOptions = [],
    range: NSRange
) -> NSRange
```

## Parameters 

`string`  

The string to search.

`options`  

The matching options to use. See NSRegularExpression.MatchingOptions for possible values.

`range`  

The range of the string to search.

## Return Value

The range of the first match. Returns `{NSNotFound, 0}` if no match is found.

## Discussion

This is a convenience method that calls enumerateMatches(in:options:range:using:).

## See Also

### Searching Strings Using Regular Expressions

func numberOfMatches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> Int

Returns the number of matches of the regular expression within the specified range of the string.

func enumerateMatches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange, using: (NSTextCheckingResult?, NSRegularExpression.MatchingFlags, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the string allowing the Block to handle each regular expression match.

func matches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> [NSTextCheckingResult]

Returns an array containing all the matches of the regular expression in the string.

func firstMatch(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> NSTextCheckingResult?

Returns the first match of the regular expression within the specified range of the string.

