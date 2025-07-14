

- SwiftUI
-  CustomAnimation 

Protocol

# CustomAnimation

A type that defines how an animatable value changes over time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@preconcurrency
protocol CustomAnimation : Hashable, Sendable
```

## Overview

Use this protocol to create a type that changes an animatable value over time, which produces a custom visual transition of a view. For example, the follow code changes an animatable value using an elastic ease-in ease-out function:

```
struct ElasticEaseInEaseOutAnimation: CustomAnimation {
    let duration: TimeInterval

    func animate(value: V, time: TimeInterval, context: inout AnimationContext) -> V? where V : VectorArithmetic {
        if time > duration { return nil } // The animation has finished.

        let p = time / duration
        let s = sin((20 * p - 11.125) * ((2 * Double.pi) / 4.5))
        if p 

Note

To maintain state during the life span of a custom animation, use the state property available on the `context` parameter value. You can also use context’s environment property to retrieve environment values from the view that created the custom animation. For more information, see AnimationContext.

To create an Animation instance of a custom animation, use the init(_:) initializer, passing in an instance of a custom animation; for example:

```
Animation(ElasticEaseInEaseOutAnimation(duration: 5.0))
```

To help make view code more readable, extend Animation and add a static property and function that returns an `Animation` instance of a custom animation. For example, the following code adds the static property `elasticEaseInEaseOut` that returns the elastic ease-in ease-out animation with a default duration of `0.35` seconds. Next, the code adds a method that returns the animation with a specified duration.

```
extension Animation {
    static var elasticEaseInEaseOut: Animation { elasticEaseInEaseOut(duration: 0.35) }
    static func elasticEaseInEaseOut(duration: TimeInterval) -> Animation {
        Animation(ElasticEaseInEaseOutAnimation(duration: duration))
    }
}
```

To animate a view with the elastic ease-in ease-out animation, a view calls either `.elasticEaseInEaseOut` or `.elasticEaseInEaseOut(duration:)`. For example, the follow code includes an Animate button that, when clicked, animates a circle as it moves from one edge of the view to the other, using the elastic ease-in ease-out animation with a duration of `5` seconds:

```
struct ElasticEaseInEaseOutView: View {
    @State private var isActive = false

    var body: some View {
        VStack(alignment: isActive ? .trailing : .leading) {
            Circle()
                .frame(width: 100.0)
                .foregroundColor(.accentColor)

            Button("Animate") {
                withAnimation(.elasticEaseInEaseOut(duration: 5.0)) {
                    isActive.toggle()
                }
            }
            .frame(maxWidth: .infinity)
        }
        .padding()
    }
}
```

 Video with custom controls. 

 Content description: A video that shows a circle that moves from one edge of the view to the other using an elastic ease-in ease-out animation. The circle's initial position is near the leading edge of the view. The circle begins moving slightly towards the leading, then towards trail edges of the view before it moves off the leading edge showing only two-thirds of the circle. The circle then moves quickly to the trailing edge of the view, going slightly beyond the edge so that only two-thirds of the circle is visible. The circle bounces back into full view before settling into position near the trailing edge of the view. The circle repeats this animation in reverse, going from the trailing edge of the view to the leading edge. 

Play 

## Topics

### Animating a value

func animate&lt;V>(value: V, time: TimeInterval, context: inout AnimationContext&lt;V>) -> V?

Calculates the value of the animation at the specified time.

**Required**

### Getting the velocity

func velocity&lt;V>(value: V, time: TimeInterval, context: AnimationContext&lt;V>) -> V?

Calculates the velocity of the animation at a specified time.

**Required** Default implementation provided.

### Determining whether to merge

func shouldMerge&lt;V>(previous: Animation, value: V, time: TimeInterval, context: inout AnimationContext&lt;V>) -> Bool

Determines whether an instance of the animation can merge with other instance of the same type.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

## See Also

### Creating custom animations

struct AnimationContext

Contextual values that a custom animation can use to manage state and access a view’s environment.

struct AnimationState

A container that stores the state for a custom animation.

protocol AnimationStateKey

A key for accessing animation state values.

struct UnitCurve

A function defined by a two-dimensional curve that maps an input progress in the range \[0,1\] to an output progress that is also in the range \[0,1\]. By changing the shape of the curve, the effective speed of an animation or other interpolation can be changed.

struct Spring

A representation of a spring’s motion.

