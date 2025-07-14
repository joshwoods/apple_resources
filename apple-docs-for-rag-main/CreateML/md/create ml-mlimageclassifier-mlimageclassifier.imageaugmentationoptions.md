

- Create ML
- MLImageClassifier
-  MLImageClassifier.ImageAugmentationOptions 

Structure

# MLImageClassifier.ImageAugmentationOptions

The variations that the training process can use to generate more training data from the training data you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
struct ImageAugmentationOptions
```

## Overview

Augmentation generates new images from the training data you supply to increase the amount of training data available to the model.

See Improving Your Model’s Accuracy for a discussion about when to use augmentation.

## Topics

### Selecting augmentation options

static let crop: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by creating cropped versions of each image.

static let rotation: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by rotating each image.

static let blur: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by blurring each image.

static let exposure: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by lightening or darkening each image.

static let noise: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by adding random amounts of noise to each image.

static let flip: MLImageClassifier.ImageAugmentationOptions

An option for augmenting training data by flipping each image along the horizontal and vertical axes.

### Creating augmentation options

init()

Creates an empty option set.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(rawValue: Int)

Creates an augmentation set with the given raw value.

let rawValue: Int

The corresponding value of the raw type.

### Testing for membership in a set

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

### Adding and removing elements

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

### Combining sets

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

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

### Comparing sets

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

### Testing for equality

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Supporting types

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias ArrayLiteralElement

The type of the elements of an array literal.

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
- Sendable
- SetAlgebra

## See Also

### Supporting types

enum FeatureExtractorType

The underlying base model that extracts image features for image classifier training session.

enum ValidationData

The source of a validation dataset for an image classifier.

