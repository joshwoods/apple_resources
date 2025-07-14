

- Core Data
- NSAttributeDescription
-  NSAttributeDescription.AttributeType 

Structure

# NSAttributeDescription.AttributeType

The types of attributes that Core Data supports.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct AttributeType
```

## Overview

Core Data attribute types explicitly distinguish between bit size. This allows their values to exist independent of the persistent store that contains them. A scalar option is available for a number of attribute types, in some cases by default.

| **Attribute type** | **Type** | **Scalar type** | **Scalar by default** |
|----|----|----|----|
| Integer 16 | NSNumber | Int16 | Yes |
| Integer 32 | NSNumber | Int32 | Yes |
| Integer 64 | NSNumber | Int64 | Yes |
| Double | NSNumber | Double | Yes |
| Float | NSNumber | Float | Yes |
| Boolean | NSNumber | Bool | Yes |
| Date | NSDate | TimeInterval | No |
| Decimal | NSDecimalNumber | NSDecimalNumber | No |
| UUID | UUID | UUID | No |
| URI | URL | — | — |
| String | String | — | — |
| Binary data | Data | — | — |
| Transformable | NSObject | — | — |
| Composite | — | — | — |
| Undefined | — | — | — |

Note

If your application uses BLOBs (binary large objects), such as image and sound files, you can choose to store their data in a location that’s external to the persistent store.

## Topics

### Attribute Types

static let binaryData: NSAttributeDescription.AttributeType

An attribute that stores binary data.

static let boolean: NSAttributeDescription.AttributeType

An attribute that stores a Boolean value.

static let composite: NSAttributeDescription.AttributeType

An attribute that derives its value by composing other attributes.

static let date: NSAttributeDescription.AttributeType

An attribute that stores a date.

static let decimal: NSAttributeDescription.AttributeType

An attribute that stores a decimal value.

static let double: NSAttributeDescription.AttributeType

An attribute that stores a double value.

static let float: NSAttributeDescription.AttributeType

An attribute that stores a float value.

static let integer16: NSAttributeDescription.AttributeType

An attribute that stores a 16-bit signed integer value.

static let integer32: NSAttributeDescription.AttributeType

An attribute that stores a 32-bit signed integer value.

static let integer64: NSAttributeDescription.AttributeType

An attribute that stores a 64-bit signed integer value.

static let objectID: NSAttributeDescription.AttributeType

An attribute that stores a managed object’s ID.

static let string: NSAttributeDescription.AttributeType

An attribute that stores a string.

static let transformable: NSAttributeDescription.AttributeType

An attribute that uses a value transformer to derive its value.

static let undefined: NSAttributeDescription.AttributeType

An attribute that doesn’t have an explicit type.

static let uri: NSAttributeDescription.AttributeType

An attribute that stores a uniform resource identifier.

static let uuid: NSAttributeDescription.AttributeType

An attribute that stores a universally unique identifier.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

## See Also

### Managing the type

var attributeValueClassName: String?

The class name that represents the attribute’s value.

var type: NSAttributeDescription.AttributeType

The attribute’s type.

var attributeType: NSAttributeType

The attribute’s type.

Deprecated

enum NSAttributeType

The types of attribute that Core Data supports.

