

- Core Media
-  CMFormatDescriptionEqualIgnoringExtensionKeys(\_:otherFormatDescription:extensionKeysToIgnore:sampleDescriptionExtensionAtomKeysToIgnore:) 

Function

# CMFormatDescriptionEqualIgnoringExtensionKeys(\_:otherFormatDescription:extensionKeysToIgnore:sampleDescriptionExtensionAtomKeysToIgnore:)

Returns a Boolean value that indicates whether two format descriptions are equal, ignoring differences in the extension keys you specify.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionEqualIgnoringExtensionKeys(
    _ formatDescription: CMFormatDescription?,
    otherFormatDescription: CMFormatDescription?,
    extensionKeysToIgnore formatDescriptionExtensionKeysToIgnore: CFTypeRef?,
    sampleDescriptionExtensionAtomKeysToIgnore: CFTypeRef?
) -> Bool
```

## Parameters 

`formatDescription`  

The first description to compare.

`otherFormatDescription`  

The second description to compare.

`formatDescriptionExtensionKeysToIgnore`  

A single format description extension key (`CFString`) or an array (`CFArray`) of keys.

`sampleDescriptionExtensionAtomKeysToIgnore`  

A single sample description extension atom key (four-character `CFString`) or an array (`CFArray`) of such keys.

## Return Value

true if the two descriptions are equal; otherwise, false.

## Discussion

When you specify any keys, the function ignores `kCMFormatDescriptionExtension_VerbatimSampleDescription` and `kCMFormatDescriptionExtension_VerbatimISOSampleEntry` for the purpose of comparison.

Note

This function is `NULL` safe.

For extension atom keys, see kCMFormatDescriptionExtension_SampleDescriptionExtensionAtoms.

## See Also

### Comparing Format Descriptions

func CMFormatDescriptionEqual(CMFormatDescription?, otherFormatDescription: CMFormatDescription?) -> Bool

Returns a Boolean value that indicates whether two format descriptions are equal.

