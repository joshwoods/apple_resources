

- Core Media
-  CMMetadataDataTypeRegistryGetBaseDataTypeForConformingDataType(\_:) 

Function

# CMMetadataDataTypeRegistryGetBaseDataTypeForConformingDataType(\_:)

Returns the base data type identifier that a data type conforms to.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataDataTypeRegistryGetBaseDataTypeForConformingDataType(_ dataType: CFString) -> CFString
```

## Parameters 

`dataType`  

Identifier of the data type to be queried.

## Return Value

Identifier of the base data type to which the given data type conforms.

## Discussion

There are a set of base data types that seed the data type registry. All valid data types will have their conformance search end with a base data type.

## See Also

### Inspecting Metadata

func CMMetadataDataTypeRegistryDataTypeIsRegistered(CFString) -> Bool

Returns a Boolean value that indicates the registration status of a data type identifier.

func CMMetadataDataTypeRegistryGetDataTypeDescription(CFString) -> CFString

Returns the data type description if it exists.

func CMMetadataDataTypeRegistryGetConformingDataTypes(CFString) -> CFArray

Returns the conforming data types for the data type, if any.

func CMMetadataDataTypeRegistryDataTypeConformsToDataType(CFString, conformsTo: CFString) -> Bool

Returns a Boolean value that indicates whether a data type conforms to another data type.

func CMMetadataDataTypeRegistryDataTypeIsBaseDataType(CFString) -> Bool

Returns a Boolean value that indicates whether a data type identifier represents a base data type.

func CMMetadataDataTypeRegistryGetBaseDataTypes() -> CFArray?

Returns an array of base data type identifiers.

