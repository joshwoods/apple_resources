

- Core Text
-  CTFontDescriptorCopyAttributes(\_:) 

Function

# CTFontDescriptorCopyAttributes(\_:)

Returns the attributes dictionary of the font descriptor.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontDescriptorCopyAttributes(_ descriptor: CTFontDescriptor) -> CFDictionary
```

## Parameters 

`descriptor`  

The font descriptor.

## Return Value

The font descriptor attributes dictionary. This dictionary contains the minimum number of attributes to specify fully this particular font descriptor.

## See Also

### Getting Attributes

func CTFontDescriptorCopyAttribute(CTFontDescriptor, CFString) -> CFTypeRef?

Returns the value associated with an arbitrary attribute.

func CTFontDescriptorCopyLocalizedAttribute(CTFontDescriptor, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?) -> CFTypeRef?

Returns a localized value for the requested attribute, if available.

