

- Core Media
-  CMFormatDescriptionGetExtension(\_:extensionKey:) 

Function

# CMFormatDescriptionGetExtension(\_:extensionKey:)

Returns an extension from the format description by using an extension key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMFormatDescriptionGetExtension(
    _ desc: CMFormatDescription,
    extensionKey: CFString
) -> CFPropertyList?
```

## Parameters 

`desc`  

The `CMFormatDescription` to examine.

`extensionKey`  

The key of the extension to return. May not be `NULL`.

## Return Value

An extension, or `NULL` if it doesn’t exist.

## Discussion

The extension is always a valid property list object. This means that it will be either a `CFNumber`, `CFString`, `CFBoolean`, `CFArray`, `CFDictionary`, `CFDate`, or `CFData`. If it’s a `CFDictionary`, the keys will all be `CFStrings`. The extension this function returns is not retained by this call, so it’s only valid as long as the `CMFormatDescription` is valid — retain it to keep it longer.

## See Also

### Inspecting Format Descriptions

func CMFormatDescriptionGetMediaType(CMFormatDescription) -> CMMediaType

Returns the media type of a format description.

func CMFormatDescriptionGetMediaSubType(CMFormatDescription) -> FourCharCode

Returns the media subtype of a format description.

func CMFormatDescriptionGetExtensions(CMFormatDescription) -> CFDictionary?

Returns all of the extensions for a format description.

func CMFormatDescriptionGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier that identifies format description objects.

