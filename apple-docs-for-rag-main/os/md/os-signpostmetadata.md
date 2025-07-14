

- os
-  SignpostMetadata 

Type Alias

# SignpostMetadata

The type that represents a message you attach to a signpost.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
typealias SignpostMetadata = OSLogMessage
```

## See Also

### Starting a Signposted Interval

func beginInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval.

func beginInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval and attaches the specified message.

func beginAnimationInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation.

func beginAnimationInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation, and attaches a message.

class OSSignpostIntervalState

An object that tracks the state of a signposted interval.

