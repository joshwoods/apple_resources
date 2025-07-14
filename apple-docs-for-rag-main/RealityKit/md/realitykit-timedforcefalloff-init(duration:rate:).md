

- RealityKit
- TimedForceFalloff
-  init(duration:rate:) 

Initializer

# init(duration:rate:)

Creates a timed force falloff.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    duration: TimeInterval,
    rate: Double = 1.0
)
```

## Parameters 

`duration`  

The lifetime of the effect in seconds.

`rate`  

Controls how fast or slow falloff occurs.

## Discussion

- When the rate is **0**, no falloff occurs. (Rigid bodies outside the bounds are culled.)

- When the rate is **greater than 0 and less than 1.0**, falloff occurs slower and is sublinear.

- When the rate is **1.0**, falloff is linear.

- When the rate is **greater than 1**, falloff occurs faster and is nonlinear.

