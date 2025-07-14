

- RealityKit
- AnimationResource
-  sequence(with:) 

Type Method

# sequence(with:)

Creates an animation resource that plays a collection of animations in a specified sequence.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func sequence(with resources: [AnimationResource]) throws -> AnimationResource
```

## Parameters 

`resources`  

The collection of animation resources to play.

## Return Value

An animation resource that plays the given array of animations.

## See Also

### Creating an animation resource

static func generate(with: any AnimationDefinition) throws -> AnimationResource

Creates an animation resource from a definition.

static func group(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that simultaneously plays back a collection of animations.

func `repeat`(count: Int) -> AnimationResource

Creates an animation that repeats the specified number of times.

func `repeat`(duration: TimeInterval) -> AnimationResource

Repeats an animation for the specified amount of time.

