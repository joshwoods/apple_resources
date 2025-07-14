

- SwiftUI
-  AnimationCompletionCriteria 

Structure

# AnimationCompletionCriteria

The criteria that determines when an animation is considered finished.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AnimationCompletionCriteria
```

## Topics

### Getting the completion criteria

static let logicallyComplete: AnimationCompletionCriteria

The animation has logically completed, but may still be in its long tail.

static let removed: AnimationCompletionCriteria

The entire animation is finished and will now be removed.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Adding state-based animation to an action

func withAnimation&lt;Result>(Animation?, () throws -> Result) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation.

func withAnimation&lt;Result>(Animation?, completionCriteria: AnimationCompletionCriteria, () throws -> Result, completion: () -> Void) rethrows -> Result

Returns the result of recomputing the view’s body with the provided animation, and runs the completion when all animations are complete.

struct Animation

The way a view changes over time to create a smooth visual transition from one state to another.

