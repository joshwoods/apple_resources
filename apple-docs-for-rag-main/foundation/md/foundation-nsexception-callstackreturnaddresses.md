

- Foundation
- NSException
-  callStackReturnAddresses 

Instance Property

# callStackReturnAddresses

The call return addresses related to a raised exception.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var callStackReturnAddresses: [NSNumber] { get }
```

## Discussion

An array of NSNumber objects encapsulating NSUInteger values. Each value is a call frame return address. The array of stack frames starts at the point at which the exception was first raised, with the first items being the most recent stack frames.

`NSException` subclasses posing as the `NSException` class or subclasses or other API elements that interfere with the exception-raising mechanism may not get this information.

## See Also

### Getting Exception Stack Frames

var callStackSymbols: [String]

An array containing the current call stack symbols.

