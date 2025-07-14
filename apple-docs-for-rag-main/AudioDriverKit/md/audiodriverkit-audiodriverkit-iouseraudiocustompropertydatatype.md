

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioCustomPropertyDataType 

Enumeration

# IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

DriverKit 21.0+

``` source
enum IOUserAudioCustomPropertyDataType : uint32_t;
```

## Discussion

Use `0` to indicate the custom property doesn’t have any data.

## Topics

### Data Types

Dictionary

A data type that indicates the custom data is a dictionary.

String

A data type that indicates the custom data is a string.

### Enumeration Cases

None

## See Also

### Creating a Custom Property

Create

Allocates and initializes an instance of the custom property class.

init

Initializes an instance of a custom property.

IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

