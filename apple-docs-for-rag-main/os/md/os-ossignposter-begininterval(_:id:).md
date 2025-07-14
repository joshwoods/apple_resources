

- os
- OSSignposter
-  beginInterval(\_:id:) 

Instance Method

# beginInterval(\_:id:)

Begins a signposted interval.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func beginInterval(
    _ name: StaticString,
    id: OSSignpostID = .exclusive
) -> OSSignpostIntervalState
```

## Parameters 

`name`  

The signpost’s name.

`id`  

The signpost’s identifier. The default value is exclusive.

## Return Value

The interval state that the signposter derives from the specified `id` parameter.

## Mentioned in 

Recording Performance Data

## Discussion

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously. If only one interval with a specific configuration can execute at any particular time, use exclusive for the `id` parameter. Otherwise, use the makeSignpostID() and makeSignpostID(from:) methods to generate a signpost identifier.

To end a signposted interval, pass the return value to one of the endInterval(_:_:) or endInterval(_:_:_:) methods. If you don’t have access to the returned interval state when you want to end the signposted interval, recreate it by passing the same signpost ID to the beginState(id:) method.

If you need to pass the returned interval state across process boundaries, you must encode it first. For more information, see OSSignpostIntervalState.

The following example demonstrates how to use a signpost ID and interval state to signpost the beginning and the end of an interval:

```
// Create a signposter that uses the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the signposted interval.
let signpostID = signposter.makeSignpostID()

// Create a name that the signposter uses, along with the 
// signpost ID, to disambiguate the begin call and end call. 
// The type must be StaticString.
let name: StaticString = "Example Signpost"

// Begin a signposted interval and keep a reference to the
// returned interval state.
let state = signposter.beginInterval(name, id: signpostID)

// Perform one or more tasks that you want to measure.

// Use the interval state from the begin call to end the
// corresponding signposted interval.
signposter.endInterval(name, state)
```

## See Also

### Starting a Signposted Interval

func beginInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval and attaches the specified message.

func beginAnimationInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation.

func beginAnimationInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation, and attaches a message.

class OSSignpostIntervalState

An object that tracks the state of a signposted interval.

typealias SignpostMetadata

The type that represents a message you attach to a signpost.

