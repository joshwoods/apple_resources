

- Foundation
- NSRegularExpression
-  escapedTemplate(for:) 

Type Method

# escapedTemplate(for:)

Returns a template string by adding backslash escapes as necessary to protect any characters that would match as pattern metacharacters

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func escapedTemplate(for string: String) -> String
```

## Parameters 

`string`  

The template string

## Return Value

The escaped template string.

## Discussion

Returns a string by adding backslash escapes as necessary to the given string, to escape any characters that would otherwise be treated as pattern metacharacters. You typically use this method to match on a particular string within a larger pattern.

For example, the string `"(N/A)"` contains the pattern metacharacters `(`, `/`, and `)`. The result of adding backslash escapes to this string is `"\\(N\\/A\\)"`.

See Flag Options for the format of the resulting template string.

## See Also

### Escaping Characters in a String

class func escapedPattern(for: String) -> String

Returns a string by adding backslash escapes as necessary to protect any characters that would match as pattern metacharacters.

