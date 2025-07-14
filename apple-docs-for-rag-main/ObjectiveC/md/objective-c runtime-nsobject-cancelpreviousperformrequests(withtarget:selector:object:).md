

- Objective-C Runtime
- NSObject
-  cancelPreviousPerformRequests(withTarget:selector:object:) 

Type Method

# cancelPreviousPerformRequests(withTarget:selector:object:)

Cancels perform requests previously registered with perform(_:with:afterDelay:).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func cancelPreviousPerformRequests(
    withTarget aTarget: Any,
    selector aSelector: Selector,
    object anArgument: Any?
)
```

## Parameters 

`aTarget`  

The target for requests previously registered with the perform(_:with:afterDelay:) instance method

`aSelector`  

The Selector for requests previously registered with the perform(_:with:afterDelay:) instance method.

`anArgument`  

The argument for requests previously registered with the perform(_:with:afterDelay:) instance method. Argument equality is determined using isEqual(_:), so the value need not be the same object that was passed originally. Pass `nil` to match a request for `nil` that was originally passed as the argument.

## Discussion

All perform requests are canceled that have the same target as `aTarget`, argument as `anArgument`, and selector as `aSelector`. This method removes perform requests only in the current run loop, not all run loops.

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

func performSelector(inBackground: Selector, with: Any?)

Invokes a method of the receiver on a new background thread.

class func cancelPreviousPerformRequests(withTarget: Any)

Cancels perform requests previously registered with the perform(_:with:afterDelay:) instance method.

