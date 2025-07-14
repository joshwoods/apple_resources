

- RealityKit
- Entity
-  pins 

Instance Property

# pins

The entity’s geometric pins.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
var pins: EntityGeometricPins { get }
```

## Discussion

You can look up, add, and remove a GeometricPin for the owning entity through this EntityGeometricPins instance. The entity’s GeometricPinsComponent stores any added geometric pins.

Other Component types on an Entity may also provide GeometricPin instances, such as for skeletal pose joints. There is no distinction between these two when GeometricPin instances are accessed.

### Geometric pins for skeletal pose joints

Entities with skeletal poses expose skeletal pose joints as GeometricPin instances. These pins are not stored in the GeometricPinsComponent on the Entity, but are obtained directly from the skeletal pose.

The name of the GeometricPin is the name of the skeletal pose joint. The pose (position and orientation) of the GeometricPin is the current pose of the joint in the coordinate frame of the Entity (i.e. *not* relative to the parent joint). While the skeletal pose is animated, the GeometricPin pose change on every frame.

The geometric pin’s name can be given as either the full skeletal pose joint path name, such as `"root/hips_joint/spine_1_joint/spine_2_joint"`, or as the leaf joint name, like `"spine_2_joint"`.

For example, get a pin via a full pose joint name, or with its leaf joint name:

```
let jointPinFromFullName = skeletalPoseEntity.pins["root/hips_joint/spine_1_joint/spine_2_joint"]
let jointPinFromShortName = skeletalPoseEntity.pins["spine_2_joint"]
```

To print all the pins, you can loop over pins.

```
for pin in skeletalPoseEntity.pins {
    print("joint   name: \(pin.name)")        // Full joint path name.
    print("    position: \(pin.position)")    // In coordinate frame of skeletalPoseEntity.
    print(" orientation: \(pin.orientation)") // In coordinate frame of skeletalPoseEntity.
}
```

In skeletal pose joint names, prefix the characters `.`, `[`, `]` and `\` with an escaping character (`\`).

For example, to access a skeletal pose joint named `"my.joint"`:

```
// To include a literal backslash in a string,
// escape it with an additional backslash.
let myJointPinEscaped = skeletalPoseEntity.pins["my\\.joint"]
// Alternatively, use Swift's raw string feature
// by enclosing the string in # symbols.
let myJointPinRaw = skeletalPoseEntity.pins[#"my\.joint"#]
```

Note

Character escaping is only required for skeletal pose joints.

