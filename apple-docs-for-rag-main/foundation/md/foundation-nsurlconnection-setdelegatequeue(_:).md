

- Foundation
- NSURLConnection
-  setDelegateQueue(\_:) 

Instance Method

# setDelegateQueue(\_:)

Determines the operation queue that is used to call methods on the connection’s delegate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setDelegateQueue(_ queue: OperationQueue?)
```

## Parameters 

`queue`  

The operation queue to use when calling delegate methods.

## Discussion

By default, a connection is scheduled on the current thread in the default mode when it is created. If you create a connection with the init(request:delegate:startImmediately:) method and provide false for the `startImmediately` parameter, you can instead schedule the connection on an operation queue before starting it with the start() method.

You cannot reschedule a connection after it has started.

It is an error to schedule delegate method calls with both this method and the schedule(in:forMode:) method.

## See Also

### Scheduling Delegate Method Calls

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Determines the run loop and mode that the connection uses to call methods on its delegate.

func unschedule(from: RunLoop, forMode: RunLoop.Mode)

Causes the connection to stop calling delegate methods in the specified run loop and mode.

