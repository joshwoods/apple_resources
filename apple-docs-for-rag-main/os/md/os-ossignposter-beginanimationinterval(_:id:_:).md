

- os
- OSSignposter
-  beginAnimationInterval(\_:id:\_:) 

Instance Method

# beginAnimationInterval(\_:id:\_:)

Begins a signposted interval for measuring an animation, and attaches a message.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func beginAnimationInterval(
    _ name: StaticString,
    id: OSSignpostID = .exclusive,
    _ message: SignpostMetadata
) -> OSSignpostIntervalState
```

## Parameters 

`name`  

The signpost’s name.

`id`  

The signpost’s identifier. The default value is exclusive.

`message`  

The interpolated string that the signposter attaches to the signpost. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Return Value

The interval state that the signposter derives from the specified `id` parameter.

## Discussion

Important

Don’t create an instance of SignpostMetadata. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously. If only one interval with a specific configuration can execute at any particular time, use exclusive for the `id` parameter. Otherwise, use the makeSignpostID() and makeSignpostID(from:) methods to generate a signpost identifier.

To end a signposted interval, pass the return value to one of the endInterval(_:_:) or endInterval(_:_:_:) methods. If you don’t have access to the returned interval state when you want to end the signposted interval, recreate it by passing the same signpost ID to the beginState(id:) method.

If you need to pass the returned interval state across process boundaries, you must encode it first. For more information, see OSSignpostIntervalState.

The following example shows how to use a signpost ID and interval state to signpost the beginning and the end of an interval that measures an animation, and also demonstrates the use of message interpolation:

```
let x: CGFloat = 0.235
let y: CGFloat = 6.12

// Create a signposter that uses the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the signposted interval.
let signpostID = signposter.makeSignpostID()

// Create a name that the signposter uses, along with the 
// signpost ID, to disambiguate the begin call and end call. 
// The type must be StaticString.
let name: StaticString = "Animation"

// Begin the signposted interval and attach a message that interpolates
// the current location of the animated object.
let state = signposter.beginAnimationInterval(name, id: signpostID,
    "x:\(x, align: .right(columns: 5)) y:\(y, align: .right(columns: 5))")

// Perform the animation that you want to measure.

// Use the interval state from the begin call to end the
// corresponding signposted interval.
signposter.endInterval(name, state)
```

## See Also

### Starting a Signposted Interval

func beginInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval.

func beginInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval and attaches the specified message.

func beginAnimationInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation.

class OSSignpostIntervalState

An object that tracks the state of a signposted interval.

typealias SignpostMetadata

The type that represents a message you attach to a signpost.

