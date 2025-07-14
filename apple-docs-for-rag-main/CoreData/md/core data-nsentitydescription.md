

- Core Data
-  NSEntityDescription 

Class

# NSEntityDescription

A description of a Core Data entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSEntityDescription
```

## Overview

Entities are to managed objects what `Class` is to `id`, or — to use a database analogy — what tables are to rows. An instance specifies the entity’s name, its attributes and relationships (as instances of NSAttributeDescription and NSRelationshipDescription) and the class that represents it. Instances of that class correspond to entries in the associated persistent store. As a minimum, an entity description requires:

- A name.

- The class name of the corresponding managed object.

If you don’t specify a class name, the framework uses NSManagedObject.

You define entities in a managed object model (an instance of NSManagedObjectModel) using Xcode’s data modeling tool. Core Data uses `NSEntityDescription` to map entries in the persistent store to managed objects in your app. It’s unlikely you’ll interact with entity descriptions directly unless you’re specifically working with models. `NSEntityDescription` provides a user dictionary for you to store any related, app-specific information.

### Editing entity descriptions

Entity descriptions are editable until an object graph manager uses them, which allows you to create or modify descriptions dynamically. However, once you associate the description’s managed object model with a persistent store coordinator, you can no longer modify it. The framework enforces this rule at runtime; any attempt to mutate the model, or any of its child objects, after you associate it with a persistent store coordinator results in an exception. If you need to modify a model that’s in use, create a copy of that model, modify it, and then discard the stale model.

If you want to create an entity hierarchy, consider the relevant API. You can only set an entity’s subentities, not an entity’s super-entity. To set an entity’s super-entity, set an array of subentities on the super entity that includes the desired entity; the entity hierarchy is built top-down.

### Using entity descriptions in dictionaries

The `copy` method of `NSEntityDescription` returns an entity such that:

```
```

Since NSDictionary copies its keys and requires that keys both conform to the NSCopying protocol and have a property that `copy` returns an object for where the source and the copy are equal, don’t use entities as keys in a dictionary. Instead, use either the entity’s name as the key or use an NSMapTable with retain callbacks.

### Fast enumeration

`NSEntityDescription` implements the NSFastEnumeration protocol. Use this to enumerate over an entity’s properties, as the following example illustrates.

```
```

## Topics

### Getting descriptive information

var name: String?

The entity name of the receiver.

var managedObjectModel: NSManagedObjectModel

The managed object model with which the receiver is associated.

var managedObjectClassName: String!

The name of the class that represents the receiver’s entity.

var renamingIdentifier: String?

The renaming identifier for the receiver.

var isAbstract: Bool

A Boolean value that indicates whether the receiver represents an abstract entity.

var userInfo: [AnyHashable : Any]?

The user info dictionary of the receiver.

var coreSpotlightDisplayNameExpression: NSExpression

The expression that computes the CoreSpotlight display name for instances of the entity.

### Managing inheritance

var subentitiesByName: [String : NSEntityDescription]

A dictionary containing the receiver’s sub-entities.

var subentities: [NSEntityDescription]

An array containing the sub-entities of the receiver.

var superentity: NSEntityDescription?

The super-entity of the receiver.

func isKindOf(entity: NSEntityDescription) -> Bool

Returns a Boolean value that indicates whether the receiver is a sub-entity of another given entity.

### Working with properties

var propertiesByName: [String : NSPropertyDescription]

A dictionary containing the properties of the receiver.

var properties: [NSPropertyDescription]

An array containing the properties of the receiver.

var attributesByName: [String : NSAttributeDescription]

The attributes of the receiver in a dictionary.

var relationshipsByName: [String : NSRelationshipDescription]

The relationships of the receiver in a dictionary.

func relationships(forDestination: NSEntityDescription) -> [NSRelationshipDescription]

Returns an array containing the relationships of the receiver where the entity description of the relationship is a given entity.

### Configuring indexes and constraints

var indexes: [NSFetchIndexDescription]

An array of fetch index descriptions for the entity.

var uniquenessConstraints: [[Any]]

An array of arrays that contains one or more attributes with a value that must be unique over the instances of that entity.

var compoundIndexes: [[Any]]

The compound indexes for the entity as an array of arrays.

Deprecated

### Creating a managed object

class func insertNewObject(forEntityName: String, into: NSManagedObjectContext) -> NSManagedObject

Creates, configures, and returns an instance of the class for the entity with a given name.

### Retrieving a description by its name

class func entity(forEntityName: String, in: NSManagedObjectContext) -> NSEntityDescription?

Returns the entity with the specified name from the managed object model associated with the specified managed object context’s persistent store coordinator.

### Managing versioning

var versionHash: Data

The version hash for the receiver.

var versionHashModifier: String?

The version hash modifier for the receiver.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Objects and entities

class NSManagedObject

The base class that all Core Data model objects inherit from.

