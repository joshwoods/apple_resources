

- SwiftUI
-  withAnimation(\_:completionCriteria:\_:completion:) 

Function

# withAnimation(\_:completionCriteria:\_:completion:)

Returns the result of recomputing the view’s body with the provided animation, and runs the completion when all animations are complete.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func withAnimation(
    _ animation: Animation? = .default,
    completionCriteria: AnimationCompletionCriteria = .logicallyComplete,
    _ body: () throws -> Result,
    completion: @escaping () -> Void
) rethrows -> Result
```

## Discussion

This function sets the given Animation as the animation property of the thread’s current Transaction as well as calling `Transaction/addAnimationCompletion` with the specified completion.

The completion callback will always be fired exactly one time. If no animations are created by the changes in `body`, then the callback will be called immediately after `body`.

## See Also

### Adding state-based animation to an action

func withAnimation&lt;Result>(Animation?, () throws -> Result) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation.

struct AnimationCompletionCriteria

The criteria that determines when an animation is considered finished.

struct Animation

The way a view changes over time to create a smooth visual transition from one state to another.

