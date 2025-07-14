

- Core Media I/O
-  CMIOExtensionPropertyAttributes 

Class

# CMIOExtensionPropertyAttributes

An object that describes the attributes of a property.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionPropertyAttributes where ObjectType : AnyObject
```

## Overview

Use a property attributes object to describe attributes such as the minimum and maximum values, discrete values, and read-only values.

## Topics

### Creating Property Attributes

init(minValue: ObjectType?, maxValue: ObjectType?, validValues: [ObjectType]?, readOnly: Bool)

Creates a property attributes object with the specified configuration.

### Inspecting Attributes

var isReadOnly: Bool

A Boolean value that indicates whether a property is read-only.

var minValue: ObjectType?

The minimum value a property supports.

var maxValue: ObjectType?

The maximum value a property supports.

var validValues: [ObjectType]?

An array of discrete values that this property supports.

### Specifying a Read-Only Attribute

class var readOnlyPropertyAttribute: CMIOExtensionPropertyAttributes&lt;AnyObject>

A class property for a read-only property attribute.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Properties

struct CMIOExtensionProperty

A structure that defines the properties that providers, devices, and streams support.

class CMIOExtensionPropertyState

An object that describes the state of a property.

let CMIOExtensionInfoDictionaryKey: String

A key that specifies the extension information dictionary.

let CMIOExtensionMachServiceNameKey: String

A key that specifies the mach service name.

