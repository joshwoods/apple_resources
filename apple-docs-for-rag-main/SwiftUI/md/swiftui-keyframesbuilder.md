

- SwiftUI
-  KeyframesBuilder 

Structure

# KeyframesBuilder

A builder that combines keyframe content values into a single value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@resultBuilder
struct KeyframesBuilder
```

## Topics

### Building keyframes

static func buildArray([some KeyframeTrackContent&lt;Value>]) -> some KeyframeTrackContent&lt;Value> 

static buildBlock()

static func buildEither&lt;First, Second>(first: First) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static func buildEither&lt;First, Second>(second: Second) -> KeyframeTrackContentBuilder&lt;Value>.Conditional&lt;Value, First, Second>

static buildExpression(_:)

Keyframes

static buildFinalResult(_:)

static buildPartialBlock(accumulated:next:)

static buildPartialBlock(first:)

## See Also

### Creating keyframe-based animation

func keyframeAnimator&lt;Value>(initialValue: Value, repeating: Bool, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Loops the given keyframes continuously, updating the view using the modifiers you apply in `body`.

func keyframeAnimator&lt;Value>(initialValue: Value, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Value) -> some View, keyframes: (Value) -> some Keyframes) -> some View

Plays the given keyframes when the given trigger value changes, updating the view using the modifiers you apply in `body`.

struct KeyframeAnimator

A container that animates its content with keyframes.

protocol Keyframes

A type that defines changes to a value over time.

struct KeyframeTimeline

A description of how a value changes over time, modeled using keyframes.

struct KeyframeTrack

A sequence of keyframes animating a single property of a root type.

struct KeyframeTrackContentBuilder

The builder that creates keyframe track content from the keyframes that you define within a closure.

protocol KeyframeTrackContent

A group of keyframes that define an interpolation curve of an animatable value.

struct CubicKeyframe

A keyframe that uses a cubic curve to smoothly interpolate between values.

struct LinearKeyframe

A keyframe that uses simple linear interpolation.

struct MoveKeyframe

A keyframe that immediately moves to the given value without interpolating.

struct SpringKeyframe

A keyframe that uses a spring function to interpolate to the given value.

