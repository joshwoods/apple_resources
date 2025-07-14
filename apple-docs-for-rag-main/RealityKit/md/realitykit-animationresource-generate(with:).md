

- RealityKit
- AnimationResource
-  generate(with:) 

Type Method

# generate(with:)

Creates an animation resource from a definition.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func generate(with definition: any AnimationDefinition) throws -> AnimationResource
```

## Parameters 

`definition`  

The configuration of a timeframe and visual semantics from which to generate an animation resource.

## Return Value

An animation resource that shares the configuration of the definition.

## See Also

### Creating an animation resource

static func sequence(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that plays a collection of animations in a specified sequence.

static func group(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that simultaneously plays back a collection of animations.

func `repeat`(count: Int) -> AnimationResource

Creates an animation that repeats the specified number of times.

func `repeat`(duration: TimeInterval) -> AnimationResource

Repeats an animation for the specified amount of time.

