

- RealityKit
- Entity animations
- OrbitAnimation
-  AnimationDefinition Implementations 

API Collection

# AnimationDefinition Implementations

## Topics

### Instance Methods

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

