

- Foundation
- NumberFormatter
-  defaultFormatterBehavior() 

Type Method

# defaultFormatterBehavior()

Returns an `NSNumberFormatterBehavior` constant that indicates default formatter behavior for new instances of `NSNumberFormatter`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func defaultFormatterBehavior() -> NumberFormatter.Behavior
```

## Return Value

An `NSNumberFormatterBehavior` constant that indicates default formatter behavior for new instances of `NSNumberFormatter`.

## See Also

### Configuring Formatter Behavior and Style

var formatterBehavior: NumberFormatter.Behavior

The formatter behavior of the receiver.

class func setDefaultFormatterBehavior(NumberFormatter.Behavior)

Sets the default formatter behavior for new instances of `NSNumberFormatter` .

var numberStyle: NumberFormatter.Style

The number style used by the receiver.

var generatesDecimalNumbers: Bool

Determines whether the receiver creates instances of NSDecimalNumber when it converts strings to number objects.

