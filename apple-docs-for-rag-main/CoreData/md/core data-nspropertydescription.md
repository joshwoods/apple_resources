

- Core Data
-  NSPropertyDescription 

Class

# NSPropertyDescription

A description of a single property belonging to an entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSPropertyDescription
```

## Overview

A property describes a single value within an object managed by the Core Data Framework. There are different types of property, each represented by a subclass which encapsulates the specific property behavior—see NSAttributeDescription, NSRelationshipDescription, and NSFetchedPropertyDescription.

Note that a property name cannot be the same as any no-parameter method name of `NSObject` or `NSManagedObject`. For example, you cannot give a property the name “description”. There are hundreds of methods on `NSObject` which may conflict with property names—and this list can grow without warning from frameworks or other libraries. You should avoid very general words (like “font”, and “color”) and words or phrases which overlap with Cocoa paradigms (such as “isEditing” and “objectSpecifier”).

Properties—relationships as well as attributes—may be transient. A managed object context knows about transient properties and tracks changes made to them. Transient properties are ignored by the persistent store, and not just during saves: you cannot fetch using a predicate based on transients (although you can use transient properties to filter in memory yourself).

### Editing Property Descriptions

Property descriptions are editable until they are used by an object graph manager (such as a persistent store coordinator). This allows you to create or modify them dynamically. However, once a description is used (when the managed object model to which it belongs is associated with a persistent store coordinator), it *must not* (indeed cannot) be changed. This is enforced at runtime: any attempt to mutate a model or any of its sub-objects after the model is associated with a persistent store coordinator causes an exception to be thrown. If you need to modify a model that is in use, create a copy, modify the copy, and then discard the objects with the old model.

## Topics

### Accessing Features of a Property

var entity: NSEntityDescription

The entity description of the receiver.

var isIndexed: Bool

A Boolean value that indicates whether the receiver should be indexed for searching.

Deprecated

var isOptional: Bool

A Boolean value that indicates whether the receiver is optional.

var isTransient: Bool

A Boolean value that indicates whether the receiver is transient.

var name: String

The name of the receiver.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

### Supporting Validation

var validationPredicates: [NSPredicate]

The validation predicates of the receiver.

var validationWarnings: [Any]

The error strings associated with the receiver’s validation predicates.

func setValidationPredicates([NSPredicate]?, withValidationWarnings: [String]?)

Sets the validation predicates and warnings of the receiver.

### Supporting Versioning

var versionHash: Data

The version hash for the receiver.

var versionHashModifier: String?

The version hash modifier for the receiver.

var renamingIdentifier: String?

The renaming identifier for the receiver.

### Specifying Spotlight Support

var isIndexedBySpotlight: Bool

A Boolean value that indicates whether Core Data adds the property’s value to the Core Spotlight index.

var isStoredInExternalRecord: Bool

A Boolean value that indicates whether to write the property’s data in an external record file that corresponds to the managed object.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSAttributeDescription
- NSExpressionDescription
- NSFetchedPropertyDescription
- NSRelationshipDescription

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

class NSAttributeDescription

A description of a single attribute belonging to an entity.

enum NSAttributeType

The types of attribute that Core Data supports.

class NSRelationshipDescription

A description of a relationship between two entities.

