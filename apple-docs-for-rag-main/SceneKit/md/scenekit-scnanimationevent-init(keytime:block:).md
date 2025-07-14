

- SceneKit
- SCNAnimationEvent
-  init(keyTime:block:) 

Initializer

# init(keyTime:block:)

Creates an animation event.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init(
    keyTime time: CGFloat,
    block eventBlock: @escaping SCNAnimationEventBlock
)
```

## Parameters 

`time`  

A number between `0.0` and `1.0` specifying the relative time for triggering the event.

`eventBlock`  

A block to call at the specified time.

## Return Value

An animation event object.

## Discussion

The `time` parameter is relative to the duration of the animation the event is attached to. For example, an event with a time of `0.5` triggers when the animation is halfway complete, and an event with a time of `1.0` triggers when the animation ends.

