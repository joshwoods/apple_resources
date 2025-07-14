

- Core Media
-  CMFormatDescriptionEqual(\_:otherFormatDescription:) 

Function

# CMFormatDescriptionEqual(\_:otherFormatDescription:)

Returns a Boolean value that indicates whether two format descriptions are equal.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionEqual(
    _ formatDescription: CMFormatDescription?,
    otherFormatDescription: CMFormatDescription?
) -> Bool
```

## Parameters 

`formatDescription`  

The first description to compare.

`otherFormatDescription`  

The second description to compare.

## Return Value

true if the two descriptions are equal; otherwise, false.

## Discussion

This calls `CFEqual` on the provided `CMFormatDescription` objects. In contrast to the Core Foundation call it is `NULL` safe.

## See Also

### Comparing Format Descriptions

func CMFormatDescriptionEqualIgnoringExtensionKeys(CMFormatDescription?, otherFormatDescription: CMFormatDescription?, extensionKeysToIgnore: CFTypeRef?, sampleDescriptionExtensionAtomKeysToIgnore: CFTypeRef?) -> Bool

Returns a Boolean value that indicates whether two format descriptions are equal, ignoring differences in the extension keys you specify.

