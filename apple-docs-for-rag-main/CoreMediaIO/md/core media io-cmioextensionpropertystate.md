

- Core Media I/O
-  CMIOExtensionPropertyState 

Class

# CMIOExtensionPropertyState

An object that describes the state of a property.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionPropertyState where ObjectType : AnyObject
```

## Overview

Create a property state object by specifying the type of data it stores, which must be a NSString, NSNumber, NSDictionary, NSArray, or NSData. You can optionally specify attributes that restrict the range of values a property allows.

## Topics

### Creating a Property State

convenience init(value: ObjectType?)

Creates a property state with a value.

init(value: ObjectType?, attributes: CMIOExtensionPropertyAttributes&lt;ObjectType>?)

Creates a property state with a value and attributes.

### Inspecting a Property State

var value: ObjectType?

The value for a property state.

var attributes: CMIOExtensionPropertyAttributes&lt;ObjectType>?

The attributes for a property state.

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

class CMIOExtensionPropertyAttributes

An object that describes the attributes of a property.

let CMIOExtensionInfoDictionaryKey: String

A key that specifies the extension information dictionary.

let CMIOExtensionMachServiceNameKey: String

A key that specifies the mach service name.

