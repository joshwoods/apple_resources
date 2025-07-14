

- Foundation
- Thread
-  isMultiThreaded() 

Type Method

# isMultiThreaded()

Returns whether the application is multithreaded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func isMultiThreaded() -> Bool
```

## Return Value

true if the application is multithreaded, otherwise false.

## Discussion

An application is considered multithreaded if a thread was ever detached from the main thread using either detachNewThreadSelector(_:toTarget:with:) or start(). If you detached a thread in your application using a non-Cocoa API, such as the POSIX or Multiprocessing Services APIs, this method could still return false. The detached thread does not have to be currently running for the application to be considered multithreaded—this method only indicates whether a single thread has been spawned.

## See Also

### Querying the Environment

class var current: Thread

Returns the thread object representing the current thread of execution.

class var callStackReturnAddresses: [NSNumber]

Returns an array containing the call stack return addresses.

class var callStackSymbols: [String]

Returns an array containing the call stack symbols.

