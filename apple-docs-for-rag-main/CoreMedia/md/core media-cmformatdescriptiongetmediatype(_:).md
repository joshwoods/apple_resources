

- Core Media
-  CMFormatDescriptionGetMediaType(\_:) 

Function

# CMFormatDescriptionGetMediaType(\_:)

Returns the media type of a format description.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionGetMediaType(_ desc: CMFormatDescription) -> CMMediaType
```

## Parameters 

`desc`  

A `CMFormatDescription` to examine.

## Return Value

A media type that identifies the format description.

## Discussion

For example, this function returns kCMMediaType_Audio for a description of an audio stream.

## See Also

### Inspecting Format Descriptions

func CMFormatDescriptionGetMediaSubType(CMFormatDescription) -> FourCharCode

Returns the media subtype of a format description.

func CMFormatDescriptionGetExtension(CMFormatDescription, extensionKey: CFString) -> CFPropertyList?

Returns an extension from the format description by using an extension key.

func CMFormatDescriptionGetExtensions(CMFormatDescription) -> CFDictionary?

Returns all of the extensions for a format description.

func CMFormatDescriptionGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier that identifies format description objects.

