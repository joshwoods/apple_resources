

- RealityKit
- AnimationResource
-  repeat(duration:) 

Instance Method

# repeat(duration:)

Repeats an animation for the specified amount of time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func `repeat`(duration: TimeInterval = .infinity) -> AnimationResource
```

## Parameters 

`duration`  

The amount of time that the animation should play. If you omit this parameter, the animation loops indefinitely.

## Return Value

A new animation resource that you play on an entity by calling the entity’s playAnimation(_:transitionDuration:startsPaused:) method.

## See Also

### Creating an animation resource

static func generate(with: any AnimationDefinition) throws -> AnimationResource

Creates an animation resource from a definition.

static func sequence(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that plays a collection of animations in a specified sequence.

static func group(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that simultaneously plays back a collection of animations.

func `repeat`(count: Int) -> AnimationResource

Creates an animation that repeats the specified number of times.

