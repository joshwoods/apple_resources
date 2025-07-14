

- Core Text
-  CTFontManagerCreateFontDescriptorFromData(\_:) 

Function

# CTFontManagerCreateFontDescriptorFromData(\_:)

Creates a font descriptor representing the font in the supplied data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontManagerCreateFontDescriptorFromData(_ data: CFData) -> CTFontDescriptor?
```

## Parameters 

`data`  

The font data.

## Return Value

A font descriptor created from the data or `NULL` if it is not a valid font.

## Discussion

If the data contains a font collection (TTC or OTC), only the first font in the collection will be returned. Use CTFontManagerCreateFontDescriptorsFromData(_:) in that case.

Note

The font descriptor returned by this function is not available through font descriptor matching. As a result, you can’t directly look for the font by name with functions like CTFontCreateWithName(_:_:_:). If you wish to make the font available for name matching, use CTFontManagerRegisterFontURLs(_:_:_:_:) instead.

## See Also

### Related Documentation

func CTFontManagerCreateFontDescriptorsFromData(CFData) -> CFArray

Creates an array of font descriptors for the fonts in the supplied data.

func CTFontManagerRegisterFontURLs(CFArray, CTFontManagerScope, Bool, ((CFArray, Bool) -> Bool)?)

Registers fonts from the specified font URLs with the font manager.

### Functions

func CTFontDescriptorMatchFontDescriptorsWithProgressHandler(CFArray, CFSet?, CTFontDescriptorProgressHandler) -> Bool

Matches font descriptors and tracks progress with a progress handler.

func CTFontManagerCompareFontFamilyNames(UnsafeRawPointer, UnsafeRawPointer, UnsafeMutableRawPointer?) -> CFComparisonResult

A comparator function to compare font family names and sort them according to Apple guidelines.

func CTFontManagerCopyAvailableFontFamilyNames() -> CFArray

Returns an array of visible font family names sorted for user interface display.

func CTFontManagerCopyAvailableFontURLs() -> CFArray

Returns an array of font URLs.

func CTFontManagerCopyAvailablePostScriptNames() -> CFArray

Returns an array of unique PostScript font names for the fonts.

func CTFontManagerCreateFontDescriptorsFromURL(CFURL) -> CFArray?

Returns an array of font descriptors representing each of the fonts in the specified URL.

func CTFontManagerCreateFontRequestRunLoopSource(CFIndex, (CFDictionary, pid_t) -> Unmanaged&lt;CFArray>) -> CFRunLoopSource?

Creates a reference to a run loop source used to convey font requests from the Font Manager.

Deprecated

func CTFontManagerEnableFontDescriptors(CFArray, Bool)

Enables or disables the matching font descriptors for font descriptor matching.

func CTFontManagerGetAutoActivationSetting(CFString?) -> CTFontManagerAutoActivationSetting

Gets the auto-activation setting for the specified bundle identifier.

func CTFontManagerGetScopeForURL(CFURL) -> CTFontManagerScope

Returns the registration scope of the specified URL.

func CTFontManagerIsSupportedFont(CFURL) -> Bool

Determines whether a file is in a supported font format.

func CTFontManagerRegisterFontsForURL(CFURL, CTFontManagerScope, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Registers fonts from the specified font URL with the Font Manager. Registered fonts are discoverable through font descriptor matching.

func CTFontManagerRegisterFontsForURLs(CFArray, CTFontManagerScope, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>?) -> Bool

Registers fonts from the specified array of font URLs with the Font Manager. Registered fonts are discoverable through font descriptor matching.

Deprecated

func CTFontManagerRegisterGraphicsFont(CGFont, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Registers the specified graphics font with the font manager.

Deprecated

func CTFontManagerSetAutoActivationSetting(CFString?, CTFontManagerAutoActivationSetting)

Sets the auto-activation setting for the specified bundle identifier.

