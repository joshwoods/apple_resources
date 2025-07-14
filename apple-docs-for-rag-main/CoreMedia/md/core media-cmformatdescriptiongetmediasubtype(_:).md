

- Core Media
-  CMFormatDescriptionGetMediaSubType(\_:) 

Function

# CMFormatDescriptionGetMediaSubType(\_:)

Returns the media subtype of a format description.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionGetMediaSubType(_ desc: CMFormatDescription) -> FourCharCode
```

## Parameters 

`desc`  

The `CMFormatDescription` to examine.

## Return Value

A media type that identifies the subtype of the `CMFormatDescription`.

## Discussion

For audio streams, the media subtype is the `asbd.mFormatID`. For video streams, the media subtype is the video codec type. For muxed streams, it’s the format of the muxed stream.

For example, the function returns `aac` for a description of an AAC audio stream, `avc1` for a description of an H.264 video stream, and `mp2t` for a description of an MPEG-2 transport (muxed) stream. If a media stream doesn’t have subtypes, this API may return `0`.

## See Also

### Inspecting Format Descriptions

func CMFormatDescriptionGetMediaType(CMFormatDescription) -> CMMediaType

Returns the media type of a format description.

func CMFormatDescriptionGetExtension(CMFormatDescription, extensionKey: CFString) -> CFPropertyList?

Returns an extension from the format description by using an extension key.

func CMFormatDescriptionGetExtensions(CMFormatDescription) -> CFDictionary?

Returns all of the extensions for a format description.

func CMFormatDescriptionGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier that identifies format description objects.

