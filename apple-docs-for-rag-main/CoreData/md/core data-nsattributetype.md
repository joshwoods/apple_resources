

- Core Data
-  NSAttributeType 

Enumeration

# NSAttributeType

The types of attribute that Core Data supports.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum NSAttributeType
```

## Mentioned in 

Configuring Attributes

## Overview

Core Data supports the following attribute types, which differentiate between bit sizes to enable data-store independence. For some types, a scalar option is available.

| **Attribute Type** | **Type** | **Scalar type** | **Scalar by default?** |
|----|----|----|----|
| Integer 16 | NSNumber | int16_t | yes |
| Integer 32 | NSNumber | int32_t | yes |
| Integer 64 | NSNumber | int64_t | yes |
| Double | NSNumber | `double` | yes |
| Float | NSNumber | `float` | yes |
| Boolean | NSNumber | BOOL | yes |
| Date | NSDate | TimeInterval | no |
| Decimal | NSDecimalNumber | NSDecimalNumber | no |
| UUID | NSUUID | NSUUID | no |
| URI | NSURL | — | — |
| String | NSString | — | — |
| Binary data | NSData | — | — |
| Transformable | NSObject | — | — |
| Composite | — | — | — |
| Undefined | — | — | — |

Note

If your application uses Binary Large Objects (BLOBs) like image and sound data, prefer to store its binary data outside of the Core Data store.

## Topics

### Attribute types

case binaryDataAttributeType

An attribute that stores binary data.

case booleanAttributeType

An attribute that stores a Boolean value.

case compositeAttributeType

An attribute that derives its value by composing other attributes.

case dateAttributeType

An attribute that stores a date.

case decimalAttributeType

An attribute that stores a decimal value.

case doubleAttributeType

An attribute that stores a double value.

case floatAttributeType

An attribute that stores a float value.

case integer16AttributeType

An attribute that stores a 16-bit signed integer value.

case integer32AttributeType

An attribute that stores a 32-bit signed integer value.

case integer64AttributeType

An attribute that stores a 64-bit signed integer value.

case objectIDAttributeType

An attribute that stores a managed object’s ID.

case stringAttributeType

An attribute that stores a string.

case transformableAttributeType

An attribute that uses a value transformer to derive its value.

case undefinedAttributeType

An attribute that doesn’t have an explicit type.

case URIAttributeType

An attribute that stores a uniform resource identifier.

case UUIDAttributeType

An attribute that stores a universally unique identifier.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Standard attributes

class NSPropertyDescription

A description of a single property belonging to an entity.

class NSAttributeDescription

A description of a single attribute belonging to an entity.

class NSRelationshipDescription

A description of a relationship between two entities.

