

- RealityKit
-  PhysicsJoints 

Structure

# PhysicsJoints

A collection of physics joints.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsJoints
```

## Topics

### Operators

static func == (PhysicsJoints, PhysicsJoints) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

Creates a new, empty collection.

init(any Sequence&lt;any PhysicsJoint>)

init(arrayLiteral: any PhysicsJoint...)

Creates an instance initialized with the given elements.

### Instance Properties

var count: Int

The number of elements in the collection.

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

let startIndex: Int

The position of the first element in a nonempty collection.

### Instance Methods

func index(after: Int) -> Int

Returns the position immediately after the given index.

func index(before: Int) -> Int

Returns the position immediately before the given index.

func replaceSubrange&lt;C>(Range&lt;Int>, with: C)

Replaces the specified subrange of elements with the given collection.

### Subscripts

subscript(Int) -> any PhysicsJoint

Accesses the element at the specified position.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Equatable Implementations

MutableCollection Implementations

RangeReplaceableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- ExpressibleByArrayLiteral
- MutableCollection
- RangeReplaceableCollection
- Sequence

## See Also

### Built-in joint types

struct PhysicsRevoluteJoint

A joint that allows one degree of rotational freedom between two entity pins, similar to a door swinging on its hinges.

struct PhysicsPrismaticJoint

A joint that allows movement along a straight line, similar to a sliding drawer.

struct PhysicsSphericalJoint

A spherical joint that allows free rotational movement between two entities’ pins.

struct PhysicsCustomJoint

A joint with six degrees of freedom that can be individually specified.

struct PhysicsDistanceJoint

A joint that maintains a minimum and maximum distance between two entity pins.

struct PhysicsFixedJoint

A joint that rigidly connects two entity pins, with zero degrees of freedom.

