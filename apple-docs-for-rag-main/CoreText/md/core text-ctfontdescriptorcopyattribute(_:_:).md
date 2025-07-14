

- Core Text
-  CTFontDescriptorCopyAttribute(\_:\_:) 

Function

# CTFontDescriptorCopyAttribute(\_:\_:)

Returns the value associated with an arbitrary attribute.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontDescriptorCopyAttribute(
    _ descriptor: CTFontDescriptor,
    _ attribute: CFString
) -> CFTypeRef?
```

## Parameters 

`descriptor`  

The font descriptor.

`attribute`  

The requested attribute.

## Return Value

A retained reference to an arbitrary attribute, or `NULL` if the requested attribute is not present.

## Discussion

Refer to Accessing Font Attributes for documentation explaining how each attribute is packaged as a CFType object.

## See Also

### Getting Attributes

func CTFontDescriptorCopyAttributes(CTFontDescriptor) -> CFDictionary

Returns the attributes dictionary of the font descriptor.

func CTFontDescriptorCopyLocalizedAttribute(CTFontDescriptor, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?) -> CFTypeRef?

Returns a localized value for the requested attribute, if available.

