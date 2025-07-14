

- Objective-C Runtime
- NSObject
-  cancelPreviousPerformRequests(withTarget:) 

Type Method

# cancelPreviousPerformRequests(withTarget:)

Cancels perform requests previously registered with the perform(_:with:afterDelay:) instance method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func cancelPreviousPerformRequests(withTarget aTarget: Any)
```

## Parameters 

`aTarget`  

The target for requests previously registered with the perform(_:with:afterDelay:) instance method.

## Discussion

All perform requests having the same target `aTarget` are canceled. This method removes perform requests only in the current run loop, not all run loops.

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

class func cancelPreviousPerformRequests(withTarget: Any, selector: Selector, object: Any?)

Cancels perform requests previously registered with perform(_:with:afterDelay:).

