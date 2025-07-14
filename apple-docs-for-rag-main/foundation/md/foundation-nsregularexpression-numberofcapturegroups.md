

- Foundation
- NSRegularExpression
-  numberOfCaptureGroups 

Instance Property

# numberOfCaptureGroups

Returns the number of capture groups in the regular expression.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var numberOfCaptureGroups: Int { get }
```

## Discussion

A capture group consists of each possible match within a regular expression. Each capture group can then be used in a replacement template to insert that value into a replacement string.

This value puts a limit on the values of `n` for `$n` in templates, and it determines the number of ranges in the returned NSTextCheckingResult instances returned in the `match...` methods.

An exception will be generated if you attempt to access a result with an index value exceeding ``` numberOfCaptureGroups``-1 ```.

## See Also

### Getting the Regular Expression and Options

var pattern: String

Returns the regular expression pattern.

var options: NSRegularExpression.Options

Returns the options used when the regular expression option was created.

