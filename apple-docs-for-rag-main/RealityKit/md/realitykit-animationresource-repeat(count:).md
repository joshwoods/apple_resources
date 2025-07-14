

- RealityKit
- AnimationResource
-  repeat(count:) 

Instance Method

# repeat(count:)

Creates an animation that repeats the specified number of times.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func `repeat`(count: Int) -> AnimationResource
```

## Parameters 

`count`  

The number of animation repetitions.

## Return Value

A repeating copy of the calling animation resource.

## See Also

### Creating an animation resource

static func generate(with: any AnimationDefinition) throws -> AnimationResource

Creates an animation resource from a definition.

static func sequence(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that plays a collection of animations in a specified sequence.

static func group(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that simultaneously plays back a collection of animations.

func `repeat`(duration: TimeInterval) -> AnimationResource

Repeats an animation for the specified amount of time.

