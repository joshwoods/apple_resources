

- Core Media
-  CMMetadataDataTypeRegistryDataTypeConformsToDataType(\_:conformsTo:) 

Function

# CMMetadataDataTypeRegistryDataTypeConformsToDataType(\_:conformsTo:)

Returns a Boolean value that indicates whether a data type conforms to another data type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMMetadataDataTypeRegistryDataTypeConformsToDataType(
    _ dataType: CFString,
    conformsTo conformsToDataType: CFString
) -> Bool
```

## Parameters 

`dataType`  

Identifier of the data type to be tested.

`conformsToDataType`  

Identifier of the data type against which to test for conformance.

## Return Value

kCFBooleanTrue if first data type conforms to the second data type; kCFBooleanFalse otherwise.

## Discussion

A given data type will conform to a second data type if any of the following are true:

1.  The data type identifiers are the same.

2.  The first data type identifier’s conformance list contains the second data type identifier.

3.  A recursive search of the conforming data types for each element in the first data type’s conformance list yields the second data type identifier.

## See Also

### Inspecting Metadata

func CMMetadataDataTypeRegistryDataTypeIsRegistered(CFString) -> Bool

Returns a Boolean value that indicates the registration status of a data type identifier.

func CMMetadataDataTypeRegistryGetDataTypeDescription(CFString) -> CFString

Returns the data type description if it exists.

func CMMetadataDataTypeRegistryGetConformingDataTypes(CFString) -> CFArray

Returns the conforming data types for the data type, if any.

func CMMetadataDataTypeRegistryDataTypeIsBaseDataType(CFString) -> Bool

Returns a Boolean value that indicates whether a data type identifier represents a base data type.

func CMMetadataDataTypeRegistryGetBaseDataTypeForConformingDataType(CFString) -> CFString

Returns the base data type identifier that a data type conforms to.

func CMMetadataDataTypeRegistryGetBaseDataTypes() -> CFArray?

Returns an array of base data type identifiers.

