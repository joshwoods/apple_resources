

- Foundation
- NumberFormatter
-  numberStyle 

Instance Property

# numberStyle

The number style used by the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var numberStyle: NumberFormatter.Style { get set }
```

## Discussion

Styles are essentially predetermined sets of values for certain properties. Examples of number-formatter styles are those used for decimal values, percentage values, and currency.

## See Also

### Configuring Formatter Behavior and Style

var formatterBehavior: NumberFormatter.Behavior

The formatter behavior of the receiver.

class func setDefaultFormatterBehavior(NumberFormatter.Behavior)

Sets the default formatter behavior for new instances of `NSNumberFormatter` .

class func defaultFormatterBehavior() -> NumberFormatter.Behavior

Returns an `NSNumberFormatterBehavior` constant that indicates default formatter behavior for new instances of `NSNumberFormatter`.

var generatesDecimalNumbers: Bool

Determines whether the receiver creates instances of NSDecimalNumber when it converts strings to number objects.

