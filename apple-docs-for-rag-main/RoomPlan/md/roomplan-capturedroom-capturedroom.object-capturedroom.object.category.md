

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  CapturedRoom.Object.Category 

Enumeration

# CapturedRoom.Object.Category

Classifications of an object in a captured room.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Category
```

## Overview

Each CapturedRoom.Object instance in a captured room’s objects array reflects a classification (category) of this type.

## Topics

### Creating an object category

init(from: any Decoder) throws

Creates an object category by deserializing the specified decoder.

### Determining the object category

case bathtub

A category for an object that represents a bathtub.

case bed

A category for an object that represents a bed.

case chair

A category for an object that represents a chair.

case dishwasher

A category for an object that represents a dishwasher.

case fireplace

A category for an object that represents a fireplace.

case oven

A category for an object that represents an oven.

case refrigerator

A category for an object that represents a refrigerator.

case sink

A category for an object that represents a sink.

case sofa

A category for an object that represents a sofa.

case stairs

A category for an object that represents stairs.

case storage

A category for an object that represents a storage area.

case stove

A category for an object that represents a stove.

case table

A category for an object that represents a table.

case television

A category for an object that represents a television.

case toilet

A category for an object that represents a toilet.

case washerDryer

A category for an object that represents a clothes washer or dryer.

### Determining supported attributes

var supportedAttributeTypes: [any CapturedRoomAttribute.Type]

Defines the attributes types compatible with a particular object category.

var supportedCombinations: [[any CapturedRoomAttribute]]

An array of supported attributes that differs by category.

func supportsCombination([any CapturedRoomAttribute]) -> Bool

Returns a Boolean value that indicates whether a category supports the given attribute combination.

### Serializing an object category

func encode(to: any Encoder) throws

Serializes an object category to the specified encoder.

### Comparing object categories

static func == (CapturedRoom.Object.Category, CapturedRoom.Object.Category) -> Bool

Determines whether two object categories are equal.

static func != (Self, Self) -> Bool

Determines whether two object categories aren’t equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [CapturedRoom.Object.Category]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Identifying an object

var identifier: UUID

A unique alphanumeric value that the framework assigns the object.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies the object’s parent object or surface.

var category: CapturedRoom.Object.Category

A classification that the captured room assigns the object.

var confidence: CapturedRoom.Confidence

A level of certainty in the object’s category.

