

- Image I/O
-  CGImageMetadataTagCreate(\_:\_:\_:\_:\_:) 

Function

# CGImageMetadataTagCreate(\_:\_:\_:\_:\_:)

Creates a new image metadata tag, and fills it with the specified information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataTagCreate(
    _ xmlns: CFString,
    _ prefix: CFString?,
    _ name: CFString,
    _ type: CGImageMetadataType,
    _ value: CFTypeRef
) -> CGImageMetadataTag?
```

## Parameters 

`xmlns`  

The namespace for the tag. Specify a common XMP namespace, such as kCGImageMetadataNamespaceExif, or a string with a custom namespace URI. A custom namespace must be a valid XML namespace. By convention, namespaces end with either the `/` or `#` character.

`prefix`  

An abbreviation for the XML namespace. You must specify a valid string for custom namespace. For standard namespaces such as kCGImageMetadataNamespaceExif, you may specify `NULL`.

`name`  

The name of the metadata tag. This string must correspond to a valid XMP name.

`type`  

The type of data in the `value` parameter. For a list of possible values, see CGImageMetadataType.

`value`  

The value of the tag. The value’s type must match the information in the `type` parameter. Supported types for this parameter are CFString, CFNumber, CFBoolean, CFArray, and CFDictionary. The keys of a dictionary must be CFString types with XMP names. The values of a dictionary must be either CFString or CGImageMetadataTag types.

The newly created tag stores only a shallow copy of the original value. As a result, modifying the original value doesn’t affect the value in the new CGImageMetadataTag.

## Return Value

A new CGImageMetadataTag type, or `NULL` if an error occurred.

