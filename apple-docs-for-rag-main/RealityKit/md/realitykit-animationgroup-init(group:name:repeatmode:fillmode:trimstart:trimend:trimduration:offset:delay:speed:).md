

- RealityKit
- AnimationGroup
-  init(group:name:repeatMode:fillMode:trimStart:trimEnd:trimDuration:offset:delay:speed:) 

Initializer

# init(group:name:repeatMode:fillMode:trimStart:trimEnd:trimDuration:offset:delay:speed:)

Creates a collection of animations that play simultaneously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    group: [any AnimationDefinition],
    name: String = "",
    repeatMode: AnimationRepeatMode = .none,
    fillMode: AnimationFillMode = [],
    trimStart: TimeInterval? = nil,
    trimEnd: TimeInterval? = nil,
    trimDuration: TimeInterval? = nil,
    offset: TimeInterval = 0,
    delay: TimeInterval = 0,
    speed: Float = 1.0
)
```

## Parameters 

`group`  

A collection of animations to run.

`name`  

A textual name for the group.

`repeatMode`  

An option that determines how the animations repeat.

`fillMode`  

The playback behavior outside of the normal duration.

`trimStart`  

The time, in seconds, at which the animations play.

`trimEnd`  

The time, in seconds, at which the animations stop.

`trimDuration`  

An optional duration that overrides the calculated duration.

`offset`  

The time, in seconds, at which the animation begins within the duration.

`delay`  

An amount of time that lapses before the animation plays.

`speed`  

A factor that increases or decreases the animation’s rate of playback.

