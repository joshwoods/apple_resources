

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.HandLocation 

Structure

# AnchoringComponent.Target.HandLocation

Defines the locations of tracked hands to look for.

Mac Catalyst 14.0+visionOS 1.0+

``` source
struct HandLocation
```

## Topics

### Structures

struct HandJoint

Describes all the hand joints.

### Operators

static func == (AnchoringComponent.Target.HandLocation, AnchoringComponent.Target.HandLocation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let aboveHand: AnchoringComponent.Target.HandLocation

An anchor location above the center of the palm in the world space, regardless how the hand is rotated.

static let indexFingerTip: AnchoringComponent.Target.HandLocation

An anchor location at the tip of the index finger.

static let palm: AnchoringComponent.Target.HandLocation

An anchor location at the center of the palm.

static let thumbTip: AnchoringComponent.Target.HandLocation

An anchor location at the tip of the thumb.

static let wrist: AnchoringComponent.Target.HandLocation

An anchor location at the center of the wrist on the back of the hand.

### Type Methods

static func joint(for: AnchoringComponent.Target.HandLocation.HandJoint) -> AnchoringComponent.Target.HandLocation

The function that returns the `HandLocation` based on `HandJoint`.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Hand tracking

Happy Beam

Leverage a Full Space to create a fun game using ARKit.

enum Chirality

Defines the chirality of tracked hands to look for.

