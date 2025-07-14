

- Foundation
- Thread
-  current 

Type Property

# current

Returns the thread object representing the current thread of execution.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var current: Thread { get }
```

## Return Value

A thread object representing the current thread of execution.

## See Also

### Related Documentation

class func detachNewThreadSelector(Selector, toTarget: Any, with: Any?)

Detaches a new thread and uses the specified selector as the thread entry point.

### Querying the Environment

class func isMultiThreaded() -> Bool

Returns whether the application is multithreaded.

class var callStackReturnAddresses: [NSNumber]

Returns an array containing the call stack return addresses.

class var callStackSymbols: [String]

Returns an array containing the call stack symbols.

