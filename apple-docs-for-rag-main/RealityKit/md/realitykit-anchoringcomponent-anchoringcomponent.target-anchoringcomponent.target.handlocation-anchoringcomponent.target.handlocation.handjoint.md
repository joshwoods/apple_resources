

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.HandLocation
-  AnchoringComponent.Target.HandLocation.HandJoint 

Structure

# AnchoringComponent.Target.HandLocation.HandJoint

Describes all the hand joints.

visionOS 2.0+

``` source
struct HandJoint
```

## Overview

For more information about the joints, refer doc://com.developer.apple/documentation/arkit/handskeleton

## Topics

### Operators

static func == (AnchoringComponent.Target.HandLocation.HandJoint, AnchoringComponent.Target.HandLocation.HandJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let forearmArm: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the elbow end of forearm on the back of hand.

static let forearmWrist: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the wrist end of forearm on the back of the hand.

static let indexFingerIntermediateBase: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate base of the index finger.

static let indexFingerIntermediateTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate tip of the index finger.

static let indexFingerKnuckle: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the knuckle of the index finger.

static let indexFingerMetacarpal: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the metacarpal of the index finger.

static let indexFingerTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the tip of the index finger.

static let littleFingerIntermediateBase: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate base of the little finger.

static let littleFingerIntermediateTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate tip of the little finger.

static let littleFingerKnuckle: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the knuckle of the little finger.

static let littleFingerMetacarpal: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the metacarpal of the little finger.

static let littleFingerTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the tip of the little finger.

static let middleFingerIntermediateBase: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate base of the middle finger.

static let middleFingerIntermediateTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate tip of the middle finger.

static let middleFingerKnuckle: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the knuckle of the middle finger.

static let middleFingerMetacarpal: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the metacarpal of the middle finger.

static let middleFingerTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the tip of the middle finger.

static let ringFingerIntermediateBase: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate base of the ring finger.

static let ringFingerIntermediateTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate tip of the ring finger.

static let ringFingerKnuckle: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the knuckle of the ring finger.

static let ringFingerMetacarpal: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the metacarpal of the ring finger.

static let ringFingerTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the tip of the ring finger.

static let thumbIntermediateBase: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate base of the thumb.

static let thumbIntermediateTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the intermediate tip of the thumb.

static let thumbKnuckle: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the knuckle of the thumb.

static let thumbTip: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the tip of the thumb.

static let wrist: AnchoringComponent.Target.HandLocation.HandJoint

An anchor location at the center of the wrist on the back of the hand.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

