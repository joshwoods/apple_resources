

- Foundation
- Thread
-  callStackReturnAddresses 

Type Property

# callStackReturnAddresses

Returns an array containing the call stack return addresses.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var callStackReturnAddresses: [NSNumber] { get }
```

## Return Value

An array containing the call stack return addresses. Each element is an `NSNumber` object containing an `NSUInteger` value.

## See Also

### Querying the Environment

class func isMultiThreaded() -> Bool

Returns whether the application is multithreaded.

class var current: Thread

Returns the thread object representing the current thread of execution.

class var callStackSymbols: [String]

Returns an array containing the call stack symbols.

