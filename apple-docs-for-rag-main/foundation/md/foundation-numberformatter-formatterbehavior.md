

- Foundation
- NumberFormatter
-  formatterBehavior 

Instance Property

# formatterBehavior

The formatter behavior of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var formatterBehavior: NumberFormatter.Behavior { get set }
```

## See Also

### Related Documentation

Data Formatting Guide

### Configuring Formatter Behavior and Style

class func setDefaultFormatterBehavior(NumberFormatter.Behavior)

Sets the default formatter behavior for new instances of `NSNumberFormatter` .

class func defaultFormatterBehavior() -> NumberFormatter.Behavior

Returns an `NSNumberFormatterBehavior` constant that indicates default formatter behavior for new instances of `NSNumberFormatter`.

var numberStyle: NumberFormatter.Style

The number style used by the receiver.

var generatesDecimalNumbers: Bool

Determines whether the receiver creates instances of NSDecimalNumber when it converts strings to number objects.

