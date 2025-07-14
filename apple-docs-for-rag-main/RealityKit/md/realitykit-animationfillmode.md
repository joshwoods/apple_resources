

- RealityKit
-  AnimationFillMode 

Structure

# AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AnimationFillMode
```

## Overview

This structure enables you to lock an animation at its starting frame for a period of time before beginning. You can also lock an animation to its ending frame for a specified amount of time after it finishes, or both.

An animation applies the fill mode you choose when a range determined by trimStart, trimEnd, or trimDuration exceeds the animation’s underlying duration, which the framework calculates as the frame count (see frames) multiplied by the frameInterval, multiplied by speed.

For example, if you set the trimStart property for an animation of a hand waving to `-1.0` and fillMode to backwards or both, the hand displays immediately, freezes at the first animation frame for one second, and then begins to wave.

## Topics

### Choosing a fill mode

static let none: AnimationFillMode

An option that indicates an animation doesn’t display frame data outside of its normal duration.

static let forwards: AnimationFillMode

An option that freezes the last frame of the animation until it stops.

static let backwards: AnimationFillMode

An option that shows the first animation frame while playback progresses to the beginning position.

static let both: AnimationFillMode

An option that displays the animation’s initial frame or final frame when playback occurs outside of the normal duration.

let rawValue: Int8

The corresponding value of the raw type.

### Creating a fill mode

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init(rawValue: Int8)

Creates a fill mode from its backing data type.

### Managing fill mode sets

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

### Comparing fill modes

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Determining the element and raw value type

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

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

### Animation definitions

struct SampledAnimation

An animation that cycles through a series of frames at a constant interval.

enum TweenMode

Options that determine whether an animation switches between frames gradually or abruptly.

struct FromToByAnimation

An animation that starts, stops, or increments by a specific value.

struct AnimationTimingFunction

The pacing of an animation transition.

struct AnimationView

An animation that represents a variation of another animation.

struct OrbitAnimation

An animation that revolves an entity around its origin.

protocol AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

