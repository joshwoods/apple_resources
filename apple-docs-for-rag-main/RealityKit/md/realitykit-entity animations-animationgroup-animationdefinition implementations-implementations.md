

- RealityKit
- Entity animations
- AnimationGroup
-  AnimationDefinition Implementations 

API Collection

# AnimationDefinition Implementations

## Topics

### Instance Methods

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeatingForever() -> Self

Repeats the animation infinitely.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

