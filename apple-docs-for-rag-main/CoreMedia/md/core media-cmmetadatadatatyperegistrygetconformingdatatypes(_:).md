

- Core Media
-  CMMetadataDataTypeRegistryGetConformingDataTypes(\_:) 

Function

# CMMetadataDataTypeRegistryGetConformingDataTypes(\_:)

Returns the conforming data types for the data type, if any.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataDataTypeRegistryGetConformingDataTypes(_ dataType: CFString) -> CFArray
```

## Parameters 

`dataType`  

Identifier of the data type to be queried.

## Return Value

List of conforming data types registered for the given data type, or `NULL` if the data type has not been registered.

## See Also

### Inspecting Metadata

func CMMetadataDataTypeRegistryDataTypeIsRegistered(CFString) -> Bool

Returns a Boolean value that indicates the registration status of a data type identifier.

func CMMetadataDataTypeRegistryGetDataTypeDescription(CFString) -> CFString

Returns the data type description if it exists.

func CMMetadataDataTypeRegistryDataTypeConformsToDataType(CFString, conformsTo: CFString) -> Bool

Returns a Boolean value that indicates whether a data type conforms to another data type.

func CMMetadataDataTypeRegistryDataTypeIsBaseDataType(CFString) -> Bool

Returns a Boolean value that indicates whether a data type identifier represents a base data type.

func CMMetadataDataTypeRegistryGetBaseDataTypeForConformingDataType(CFString) -> CFString

Returns the base data type identifier that a data type conforms to.

func CMMetadataDataTypeRegistryGetBaseDataTypes() -> CFArray?

Returns an array of base data type identifiers.

