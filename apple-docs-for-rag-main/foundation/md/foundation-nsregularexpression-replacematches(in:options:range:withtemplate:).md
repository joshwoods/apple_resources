

- Foundation
- NSRegularExpression
-  replaceMatches(in:options:range:withTemplate:) 

Instance Method

# replaceMatches(in:options:range:withTemplate:)

Replaces regular expression matches within the mutable string using the template string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceMatches(
    in string: NSMutableString,
    options: NSRegularExpression.MatchingOptions = [],
    range: NSRange,
    withTemplate templ: String
) -> Int
```

## Parameters 

`string`  

The mutable string to search and replace values within.

`options`  

The matching options to use. See NSRegularExpression.MatchingOptions for possible values.

`range`  

The range of the string to search.

`templ`  

The substitution template used when replacing matching instances.

## Return Value

The number of matches.

## Discussion

See Flag Options for the format of `templ`.

## See Also

### Replacing Strings Using Regular Expressions

func stringByReplacingMatches(in: String, options: NSRegularExpression.MatchingOptions, range: NSRange, withTemplate: String) -> String

Returns a new string containing matching regular expressions replaced with the template string.

