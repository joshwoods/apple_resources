

- Foundation
- NSDecimalNumberHandler
-  default 

Type Property

# default

Returns the default instance of `NSDecimalNumberHandler`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: NSDecimalNumberHandler { get }
```

## Return Value

The default instance of `NSDecimalNumberHandler`.

## Discussion

This default decimal number handler rounds to the closest possible return value. It assumes your need for precision does not exceed 38 significant digits, and it raises an exception when its `NSDecimalNumber` object tries to divide by `0` or when its `NSDecimalNumber` object produces a number too big or too small to be represented.

## See Also

### Related Documentation

Number and Value Programming Topics

