

- Foundation
- NSRegularExpression
-  matches(in:options:range:) 

Instance Method

# matches(in:options:range:)

Returns an array containing all the matches of the regular expression in the string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func matches(
    in string: String,
    options: NSRegularExpression.MatchingOptions = [],
    range: NSRange
) -> [NSTextCheckingResult]
```

## Parameters 

`string`  

The string to search.

`options`  

The matching options to use. See NSRegularExpression.MatchingOptions for possible values.

`range`  

The range of the string to search.

## Return Value

An array of NSTextCheckingResult objects. Each result gives the overall matched range via its range property, and the range of each individual capture group via its range(at:) method. The range {`NSNotFound`, 0} is returned if one of the capture groups did not participate in this particular match.

## Discussion

This is a convenience method that calls enumerateMatches(in:options:range:using:) passing the appropriate string, options, and range.

## See Also

### Searching Strings Using Regular Expressions

func numberOfMatches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> Int

Returns the number of matches of the regular expression within the specified range of the string.

func enumerateMatches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange, using: (NSTextCheckingResult?, NSRegularExpression.MatchingFlags, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates the string allowing the Block to handle each regular expression match.

func firstMatch(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> NSTextCheckingResult?

Returns the first match of the regular expression within the specified range of the string.

func rangeOfFirstMatch(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange) -> NSRange

Returns the range of the first match of the regular expression within the specified range of the string.

