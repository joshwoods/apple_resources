

- os
-  OSSignpostIntervalState 

Class

# OSSignpostIntervalState

An object that tracks the state of a signposted interval.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class OSSignpostIntervalState
```

## Overview

OSSignposter uses interval state to enforce the following runtime assertions:

- Multiple end calls don’t consume the same interval state.

- The begin call and end call use the same name.

- The begin call and end call emit signposts to the same underlying log.

- You don’t use the exclusive signpost ID for intervals that cross process boundaries.

In debug builds, any assertion failures result in a crash. In production builds, your app continues to run and, instead, the signposter attaches an error message to the interval’s closing signpost.

OSSignpostIntervalState adopts the Codable protocol, which means you can serialize state and safely share it across processes, as the following example shows:

```
// A closure that represents a process in the context of this example.
let processA: () throws -> Data = {
    // Create a signposter that uses the default subsystem.
    let signposter = OSSignposter()

    // Generate a signpost ID to associate with the signposted interval.
    let signpostID = signposter.makeSignpostID()

    // Begin a signposted interval.
    let state = signposter.beginInterval("Example", id: signpostID)

    // Encode the state into JSON and return to the caller.
    return try JSONEncoder().encode(state)
}

// A closure that represents a different process.
let processB: (Data) throws -> Void = { data in
    // Decode the provided JSON data into an instance of 
    // OSSignpostIntervalState.
    let state = try JSONDecoder().decode(OSSignpostIntervalState.self, 
        from: data)

    // Create a signposter that uses the same subsystem as
    // the original, which, in this case, is the default.
    let signposter = OSSignposter()

    // End the signposted interval using the decoded state.
    signposter.endInterval("Example", state)
}

// Execute the two closures.
do {
    let data = try processA()
    try processB(data)
} catch {
    // Handle any thrown errors accordingly.
}
```

If you don’t have access to the returned interval state from the call that begins the signposted interval, or the cost you incur when serializing the state to pass between processes is unacceptable, recreate the interval state by passing the interval’s signpost ID to the beginState(id:) method.

## Topics

### Creating Interval State

init(from: any Decoder) throws

Decodes the interval state from the provided decoder.

### Recreating Interval State

static func beginState(id: OSSignpostID) -> OSSignpostIntervalState

Recreates interval state from the specified signpost ID.

### Encoding Interval State

func encode(to: any Encoder) throws

Encodes the interval state into the provided encoder.

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

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

typealias SignpostMetadata

The type that represents a message you attach to a signpost.

