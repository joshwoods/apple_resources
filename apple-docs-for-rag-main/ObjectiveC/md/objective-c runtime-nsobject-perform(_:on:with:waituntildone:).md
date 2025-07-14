

- Objective-C Runtime
- NSObject
-  perform(\_:on:with:waitUntilDone:) 

Instance Method

# perform(\_:on:with:waitUntilDone:)

Invokes a method of the receiver on the specified thread using the default mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func perform(
    _ aSelector: Selector,
    on thr: Thread,
    with arg: Any?,
    waitUntilDone wait: Bool
)
```

## Parameters 

`aSelector`  

A Selector that identifies the method to invoke. The method should not have a significant return value and should take a single argument of type id, or no arguments.

`thr`  

The thread on which to execute `aSelector`.

`arg`  

The argument to pass to the method when it is invoked. Pass `nil` if the method does not take an argument.

`wait`  

A Boolean that specifies whether the current thread blocks until after the specified selector is performed on the receiver on the specified thread. Specify YES to block this thread; otherwise, specify NO to have this method return immediately.

If the current thread and target thread are the same, and you specify YES for this parameter, the selector is performed immediately on the current thread. If you specify NO, this method queues the message on the thread’s run loop and returns, just like it does for other threads. The current thread must then dequeue and process the message when it has an opportunity to do so.

## Discussion

You can use this method to deliver messages to other threads in your application. The message in this case is a method of the current object that you want to execute on the target thread.

This method queues the message on the run loop of the target thread using the default run loop modes—that is, the modes associated with the common constant. As part of its normal run loop processing, the target thread dequeues the message (assuming it is running in one of the default run loop modes) and invokes the desired method.

You cannot cancel messages queued using this method. If you want the option of canceling a message on the current thread, you must use either the perform(_:with:afterDelay:) or perform(_:with:afterDelay:inModes:) method.

### Special Considerations

This method registers with the runloop of its current context, and depends on that runloop being run on a regular basis to perform correctly. One common context where you might call this method and end up registering with a runloop that is not automatically run on a regular basis is when being invoked by a dispatch queue. If you need this type of functionality when running on a dispatch queue, you should use dispatch_after and related methods to get the behavior you want.

## See Also

### Sending Messages

func perform(Selector, with: Any?, afterDelay: TimeInterval)

Invokes a method of the receiver on the current thread using the default mode after a delay.

func perform(Selector, with: Any?, afterDelay: TimeInterval, inModes: [RunLoop.Mode])

Invokes a method of the receiver on the current thread using the specified modes after a delay.

func performSelector(onMainThread: Selector, with: Any?, waitUntilDone: Bool)

Invokes a method of the receiver on the main thread using the default mode.

func performSelector(onMainThread: Selector, with: Any?, waitUntilDone: Bool, modes: [String]?)

Invokes a method of the receiver on the main thread using the specified modes.

func perform(Selector, on: Thread, with: Any?, waitUntilDone: Bool, modes: [String]?)

Invokes a method of the receiver on the specified thread using the specified modes.

func performSelector(inBackground: Selector, with: Any?)

Invokes a method of the receiver on a new background thread.

class func cancelPreviousPerformRequests(withTarget: Any)

Cancels perform requests previously registered with the perform(_:with:afterDelay:) instance method.

class func cancelPreviousPerformRequests(withTarget: Any, selector: Selector, object: Any?)

Cancels perform requests previously registered with perform(_:with:afterDelay:).

