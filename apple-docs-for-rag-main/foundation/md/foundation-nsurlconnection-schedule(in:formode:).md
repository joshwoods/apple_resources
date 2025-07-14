

- Foundation
- NSURLConnection
-  schedule(in:forMode:) 

Instance Method

# schedule(in:forMode:)

Determines the run loop and mode that the connection uses to call methods on its delegate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func schedule(
    in aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aRunLoop`  

The RunLoop instance to use when calling delegate methods.

`mode`  

The mode in which to call delegate methods.

## Discussion

By default, a connection is scheduled on the current thread in the default mode when it is created. If you create a connection with the init(request:delegate:startImmediately:) method and provide false for the `startImmediately` parameter, you can schedule the connection on a different run loop or mode before starting it with the start() method. You can schedule a connection on multiple run loops and modes, or on the same run loop in multiple modes.

You cannot reschedule a connection after it has started.

It is an error to schedule delegate method calls with both this method and the setDelegateQueue(_:) method.

## See Also

### Scheduling Delegate Method Calls

func setDelegateQueue(OperationQueue?)

Determines the operation queue that is used to call methods on the connection’s delegate.

func unschedule(from: RunLoop, forMode: RunLoop.Mode)

Causes the connection to stop calling delegate methods in the specified run loop and mode.

