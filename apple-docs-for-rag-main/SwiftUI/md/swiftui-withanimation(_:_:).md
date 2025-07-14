

- SwiftUI
-  withAnimation(\_:\_:) 

Function

# withAnimation(\_:\_:)

Returns the result of recomputing the view’s body with the provided animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withAnimation(
    _ animation: Animation? = .default,
    _ body: () throws -> Result
) rethrows -> Result
```

## Mentioned in 

Managing user interface state

## Discussion

This function sets the given Animation as the animation property of the thread’s current Transaction.

## See Also

### Adding state-based animation to an action

func withAnimation&lt;Result>(Animation?, completionCriteria: AnimationCompletionCriteria, () throws -> Result, completion: () -> Void) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation, and runs the completion when all animations are complete.

struct AnimationCompletionCriteria

The criteria that determines when an animation is considered finished.

struct Animation

The way a view changes over time to create a smooth visual transition from one state to another.

