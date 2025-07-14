

- Core Media
-  CMFormatDescriptionGetTypeID() 

Function

# CMFormatDescriptionGetTypeID()

Returns the Core Foundation type identifier that identifies format description objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionGetTypeID() -> CFTypeID
```

## Discussion

You can check if a `CFTypeRef` object is a `CMFormatDescription` by comparing CFGetTypeID(object) with `CMFormatDescriptionGetTypeID`().

## See Also

### Inspecting Format Descriptions

func CMFormatDescriptionGetMediaType(CMFormatDescription) -> CMMediaType

Returns the media type of a format description.

func CMFormatDescriptionGetMediaSubType(CMFormatDescription) -> FourCharCode

Returns the media subtype of a format description.

func CMFormatDescriptionGetExtension(CMFormatDescription, extensionKey: CFString) -> CFPropertyList?

Returns an extension from the format description by using an extension key.

func CMFormatDescriptionGetExtensions(CMFormatDescription) -> CFDictionary?

Returns all of the extensions for a format description.

