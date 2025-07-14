

- RealityKit
- BillboardAction
-  BillboardAction.Transition 

Structure

# BillboardAction.Transition

The duration and timing of how an action event transitions from one state to another.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Transition
```

## Topics

### Initializers

init(duration: TimeInterval, timingFunction: AnimationTimingFunction)

Creates a transition with a duration and timing function.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var duration: TimeInterval

The amount of time the transition takes to go from one state to another.

var timingFunction: AnimationTimingFunction

The rate of change at the beginning and end of the transition.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

## Relationships

### Conforms To

- Decodable
- Encodable

