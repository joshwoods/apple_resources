

- Core Data
-  NSAttributeDescription 

Class

# NSAttributeDescription

A description of a single attribute belonging to an entity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSAttributeDescription
```

## Overview

`NSAttributeDescription` inherits from NSPropertyDescription, which provides most of the basic behavior. Instances of `NSAttributeDescription` are used to describe attributes, as distinct from relationships. The class adds the ability to specify the attribute type, and to specify a default value. In a managed object model, you must specify the type of all attributes—you can only use the undefined attribute type (`NSUndefinedAttributeType`) for transient attributes.

### Editing Attribute Descriptions

Attribute descriptions are editable until they are used by an object graph manager. This allows you to create or modify them dynamically. However, once a description is used (when the managed object model to which it belongs is associated with a persistent store coordinator), it *must not* (indeed cannot) be changed. This is enforced at runtime: any attempt to mutate a model or any of its sub-objects after the model is associated with a persistent store coordinator causes an exception to be thrown. If you need to modify a model that is in use, create a copy, modify the copy, and then discard the objects with the old model.

Note

Default values set for attributes are retained by a managed object model, not copied. This means that attribute values do not have to implement the `NSCopying` protocol, however it also means that you should not modify any objects after they have been set as default values.

## Topics

### Managing the type

var attributeValueClassName: String?

The class name that represents the attribute’s value.

var type: NSAttributeDescription.AttributeType

The attribute’s type.

struct AttributeType

The types of attributes that Core Data supports.

var attributeType: NSAttributeType

The attribute’s type.

Deprecated

enum NSAttributeType

The types of attribute that Core Data supports.

### Configuring the behavior

var allowsCloudEncryption: Bool

A Boolean value that determines whether to encrypt the attribute’s value.

var allowsExternalBinaryDataStorage: Bool

A Boolean value that indicates whether the attribute allows external binary storage.

var defaultValue: Any?

The default value of the attribute.

var preservesValueInHistoryOnDeletion: Bool

A Boolean value that indicates whether the attribute records its value in the persistent history transaction for a managed object’s deletion.

var valueTransformerName: String?

The name of the transformer to use for the attribute value.

### Getting version information

var versionHash: Data

The version hash for the attribute.

### Deprecated

Deprecated symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSPropertyDescription

### Inherited By

- NSCompositeAttributeDescription
- NSDerivedAttributeDescription

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

enum NSAttributeType

The types of attribute that Core Data supports.

class NSRelationshipDescription

A description of a relationship between two entities.

