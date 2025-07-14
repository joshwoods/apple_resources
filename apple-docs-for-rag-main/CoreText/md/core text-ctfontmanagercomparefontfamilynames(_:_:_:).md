

- Core Text
-  CTFontManagerCompareFontFamilyNames(\_:\_:\_:) 

Function

# CTFontManagerCompareFontFamilyNames(\_:\_:\_:)

A comparator function to compare font family names and sort them according to Apple guidelines.

macOS 10.6+

``` source
func CTFontManagerCompareFontFamilyNames(
    _ family1: UnsafeRawPointer,
    _ family2: UnsafeRawPointer,
    _ context: UnsafeMutableRawPointer?
) -> CFComparisonResult
```

## Parameters 

`family1`  

The first localized font family name to compare, as a `CFStringRef` object.

`family2`  

The second localized font family name to compare, as a `CFStringRef` object.

`context`  

Unused. Can be `NULL`.

## Return Value

A `CFComparisonResult` value indicating the sort order for the two family names. `kCFComparisonResultGreatherThan` if `family1` is greater than `family2`, `kCFComparisonResultLessThan` if `family1` is less than `family2`, and `kCFComparisonResultEqualTo` if they are equal.

## Discussion

This `CFComparatorFunction` function compares font family names and sorts them in the Apple preferred order, accounting for foundry prefix. Family names with recognized prefixes are sorted after the unprefixed names in prefix order.

## See Also

### Functions

func CTFontDescriptorMatchFontDescriptorsWithProgressHandler(CFArray, CFSet?, CTFontDescriptorProgressHandler) -> Bool

Matches font descriptors and tracks progress with a progress handler.

func CTFontManagerCopyAvailableFontFamilyNames() -> CFArray

Returns an array of visible font family names sorted for user interface display.

func CTFontManagerCopyAvailableFontURLs() -> CFArray

Returns an array of font URLs.

func CTFontManagerCopyAvailablePostScriptNames() -> CFArray

Returns an array of unique PostScript font names for the fonts.

func CTFontManagerCreateFontDescriptorFromData(CFData) -> CTFontDescriptor?

Creates a font descriptor representing the font in the supplied data.

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

