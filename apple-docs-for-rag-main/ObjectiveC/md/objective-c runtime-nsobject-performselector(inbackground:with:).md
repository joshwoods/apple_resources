

- Objective-C Runtime
- NSObject
-  performSelector(inBackground:with:) 

Instance Method

# performSelector(inBackground:with:)

Invokes a method of the receiver on a new background thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func performSelector(
    inBackground aSelector: Selector,
    with arg: Any?
)
```

## Parameters 

`aSelector`  

A Selector that identifies the method to invoke. The method should not have a significant return value and should take a single argument of type id, or no arguments.

`arg`  

The argument to pass to the method when it is invoked. Pass `nil` if the method does not take an argument.

## Discussion

This method creates a new thread in your application, putting your application into multithreaded mode if it was not already. The method represented by `aSelector` must set up the thread environment just as you would for any other new thread in your program. For more information about how to configure and run threads, see Threading Programming Guide.

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

func perform(Selector, on: Thread, with: Any?, waitUntilDone: Bool)

Invokes a method of the receiver on the specified thread using the default mode.

func perform(Selector, on: Thread, with: Any?, waitUntilDone: Bool, modes: [String]?)

Invokes a method of the receiver on the specified thread using the specified modes.

class func cancelPreviousPerformRequests(withTarget: Any)

Cancels perform requests previously registered with the perform(_:with:afterDelay:) instance method.

class func cancelPreviousPerformRequests(withTarget: Any, selector: Selector, object: Any?)

Cancels perform requests previously registered with perform(_:with:afterDelay:).

