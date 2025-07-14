

- RealityKit
- ARView
-  ARView.DebugOptions 

Structure

# ARView.DebugOptions

Options for drawing overlay content in a scene that can aid in debugging.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
struct DebugOptions
```

## Topics

### Configuring debug options

static let none: ARView.DebugOptions

Disable all debugging overlays.

static let showPhysics: ARView.DebugOptions

Draw visualizations for collision objects and rigid bodies.

static let showStatistics: ARView.DebugOptions

Collect performance statistics and display them in the view.

static let showAnchorOrigins: ARView.DebugOptions

Display anchor origins.

static let showAnchorGeometry: ARView.DebugOptions

Display anchor geometry.

static let showWorldOrigin: ARView.DebugOptions

Display a coordinate axis indicating the position and orientation of the AR world coordinate system.

static let showFeaturePoints: ARView.DebugOptions

Display a point cloud showing intermediate results of the scene analysis used to track device position.

static let showSceneUnderstanding: ARView.DebugOptions

Display the depth-colored wireframe for scene-understanding meshes.

### Creating a debug option set

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: Int)

Create a debug options enumeration from a raw value.

let rawValue: Int

Options for drawing overlay content in a scene that aids in debugging the scene.

### Testing for membership in a debug option set

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

### Adding and removing options

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

### Combining options

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

### Comparing options

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### UIKit and AppKit presentation

class ARView

A view that enables you to display an AR experience with RealityKit.

typealias ARViewBase

The platform-specific base class for the view into which RealityKit renders content.

