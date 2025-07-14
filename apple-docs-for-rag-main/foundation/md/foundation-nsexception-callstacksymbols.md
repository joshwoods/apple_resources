

- Foundation
- NSException
-  callStackSymbols 

Instance Property

# callStackSymbols

An array containing the current call stack symbols.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var callStackSymbols: [String] { get }
```

## Discussion

An array of strings describing the call stack backtrace at the moment the exception was first raised. The format of each string is determined by the `backtrace_symbols()` API

## See Also

### Getting Exception Stack Frames

var callStackReturnAddresses: [NSNumber]

The call return addresses related to a raised exception.

