

- Foundation
- NSRegularExpression
-  options 

Instance Property

# options

Returns the options used when the regular expression option was created.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var options: NSRegularExpression.Options { get }
```

## Discussion

The options property specifies aspects of the regular expression matching that are always used when matching the regular expression. For example, if the expression is case sensitive, allows comments, ignores metacharacters, etc. See NSRegularExpression.Options for a complete discussion of the possible constants and their meanings.

## See Also

### Related Documentation

init(pattern: String, options: NSRegularExpression.Options) throws

Returns an initialized NSRegularExpression instance with the specified regular expression pattern and options.

### Getting the Regular Expression and Options

var pattern: String

Returns the regular expression pattern.

var numberOfCaptureGroups: Int

Returns the number of capture groups in the regular expression.

