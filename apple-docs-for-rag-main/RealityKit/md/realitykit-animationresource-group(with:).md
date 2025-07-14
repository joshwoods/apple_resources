

- RealityKit
- AnimationResource
-  group(with:) 

Type Method

# group(with:)

Creates an animation resource that simultaneously plays back a collection of animations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func group(with resources: [AnimationResource]) throws -> AnimationResource
```

## Parameters 

`resources`  

The collection of animation resources to play back.

## Return Value

An animation resource that simultaneously plays back the argument collection of animations.

## See Also

### Creating an animation resource

static func generate(with: any AnimationDefinition) throws -> AnimationResource

Creates an animation resource from a definition.

static func sequence(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that plays a collection of animations in a specified sequence.

func `repeat`(count: Int) -> AnimationResource

Creates an animation that repeats the specified number of times.

func `repeat`(duration: TimeInterval) -> AnimationResource

Repeats an animation for the specified amount of time.

