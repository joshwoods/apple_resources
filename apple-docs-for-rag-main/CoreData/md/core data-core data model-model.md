

- Core Data
-  Core Data model 

API Collection

# Core Data model

Describe your app’s object structure.

## Overview

In most cases, you describe your app’s data model using Xcode’s data model editor. NSManagedObjectModel represents the `.xcdatamodeld` file in your project’s source list. This is where you define entities that you use to generate NSManagedObject subclasses for Core Data to manage.

The entities you create are NSEntityDescription instances. Entities’ properties are subclasses of NSPropertyDescription, namely NSAttributeDescription for attributes, NSRelationshipDescription for relationships, and NSFetchedPropertyDescription for fetched properties.

The various attribute types are enumerated in NSAttributeType.

## Topics

### Objects and entities

class NSManagedObject

The base class that all Core Data model objects inherit from.

class NSEntityDescription

A description of a Core Data entity.

### Standard attributes

class NSPropertyDescription

A description of a single property belonging to an entity.

class NSAttributeDescription

A description of a single attribute belonging to an entity.

enum NSAttributeType

The types of attribute that Core Data supports.

class NSRelationshipDescription

A description of a relationship between two entities.

### Computed attributes

class NSCompositeAttributeDescription

A description of an attribute that derives its value by composing other attributes.

class NSDerivedAttributeDescription

A description of an attribute that derives its value by performing a calculation on a related attribute.

### Fetched properties

class NSFetchedPropertyDescription

A description object used to define which properties are fetched from Core Data.

## See Also

### Data modeling

Modeling data

Configure the data model file to contain your app’s object graph.

