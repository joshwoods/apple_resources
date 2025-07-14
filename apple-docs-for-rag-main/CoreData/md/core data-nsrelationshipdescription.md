

- Core Data
-  NSRelationshipDescription 

Class

# NSRelationshipDescription

A description of a relationship between two entities.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSRelationshipDescription
```

## Overview

NSRelationshipDescription provides additional attributes that are specific to modeling a relationship between two entities. For the common attributes of all property types, see NSPropertyDescription.

For example, use this class to define a relationship’s *cardinality* — the number of managed objects the relationship can reference.

- For a to-one relationship, set maxCount to `1`.

- For a to-many relationship, set maxCount to a number greater than `1` to impose an upper limit; otherwise, use `0` to allow an unlimited number of referenced objects.

At runtime, you can modify a relationship description until you associate its owning managed object model with a persistent store coordinator. If you attempt to modify the model after you associate it, Core Data throws an exception. To modify a model that’s in use, create and modify a copy and then discard any objects that belong to the original model.

## Topics

### Configuring the Destination

var inverseRelationship: NSRelationshipDescription?

The relationship that represents the inverse of the current relationship.

var destinationEntity: NSEntityDescription?

The type of object the relationship contains.

var isOrdered: Bool

A Boolean value that determines whether the relationship preserves the order of the referenced managed objects.

### Configuring Cardinality

var isToMany: Bool

Returns a Boolean value that indicates whether the relationship can contain many managed objects.

var minCount: Int

The minimum number of managed objects the relationship can reference.

var maxCount: Int

The maximum number of managed objects the relationship can reference.

### Configuring Delete Behavior

var deleteRule: NSDeleteRule

The rule to apply when you delete the relationship’s owning managed object.

enum NSDeleteRule

Constants that determine what happens when you delete a relationship’s owning managed object.

### Getting Version Data

var versionHash: Data

The relationship’s unique identity.

## Relationships

### Inherits From

- NSPropertyDescription

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Standard attributes

class NSPropertyDescription

A description of a single property belonging to an entity.

class NSAttributeDescription

A description of a single attribute belonging to an entity.

enum NSAttributeType

The types of attribute that Core Data supports.

