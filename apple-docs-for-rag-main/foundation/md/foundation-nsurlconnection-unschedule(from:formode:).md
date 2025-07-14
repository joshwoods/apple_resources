

- Foundation
- NSURLConnection
-  unschedule(from:forMode:) 

Instance Method

# unschedule(from:forMode:)

Causes the connection to stop calling delegate methods in the specified run loop and mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unschedule(
    from aRunLoop: RunLoop,
    forMode mode: RunLoop.Mode
)
```

## Parameters 

`aRunLoop`  

The run loop instance to unschedule.

`mode`  

The mode to unschedule.

## Discussion

By default, a connection is scheduled on the current thread in the default mode when it is created. If you create a connection with the init(request:delegate:startImmediately:) method and provide false for the `startImmediately` parameter, you can instead schedule connection on a different run loop or mode before starting it with the start() method. You can schedule a connection on multiple run loops and modes, or on the same run loop in multiple modes. Use this method to unschedule the connection from an undesired run loop and mode before starting the connection.

You cannot reschedule a connection after it has started. It is not necessary to unschedule a connection after it has finished.

## See Also

### Scheduling Delegate Method Calls

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Determines the run loop and mode that the connection uses to call methods on its delegate.

func setDelegateQueue(OperationQueue?)

Determines the operation queue that is used to call methods on the connection’s delegate.

