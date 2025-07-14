

- Foundation
- NSRegularExpression
-  escapedPattern(for:) 

Type Method

# escapedPattern(for:)

Returns a string by adding backslash escapes as necessary to protect any characters that would match as pattern metacharacters.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func escapedPattern(for string: String) -> String
```

## Parameters 

`string`  

The string.

## Return Value

The escaped string.

## Discussion

Returns a string by adding backslash escapes as necessary to the given string, to escape any characters that would otherwise be treated as pattern metacharacters. You typically use this method to match on a particular string within a larger pattern.

For example, the string `"(N/A)"` contains the pattern metacharacters `(`, `/`, and `)`. The result of adding backslash escapes to this string is `"\\(N\\/A\\)"`.

## See Also

### Escaping Characters in a String

class func escapedTemplate(for: String) -> String

Returns a template string by adding backslash escapes as necessary to protect any characters that would match as pattern metacharacters

