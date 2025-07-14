

- SwiftUI
- SpringKeyframe
-  init(\_:duration:spring:startVelocity:) 

Initializer

# init(\_:duration:spring:startVelocity:)

Creates a new keyframe using the given value and timestamp.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ to: Value,
    duration: TimeInterval? = nil,
    spring: Spring = Spring(),
    startVelocity: Value? = nil
)
```

## Parameters 

`to`  

The value of the keyframe.

`duration`  

The duration of the segment defined by this keyframe, or nil to use the settling duration of the spring.

`spring`  

The spring that defines the shape of the segment befire this keyframe

`startVelocity`  

The velocity of the value at the start of the segment, or `nil` to automatically compute the velocity to maintain smooth motion.

