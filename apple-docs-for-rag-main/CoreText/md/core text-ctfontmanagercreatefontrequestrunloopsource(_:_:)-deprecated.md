

- Core Text
-  CTFontManagerCreateFontRequestRunLoopSource(\_:\_:) Deprecated

Function

# CTFontManagerCreateFontRequestRunLoopSource(\_:\_:)

Creates a reference to a run loop source used to convey font requests from the Font Manager.

macOS 10.6–11.0Deprecated

``` source
func CTFontManagerCreateFontRequestRunLoopSource(
    _ sourceOrder: CFIndex,
    _ createMatchesCallback: @escaping (CFDictionary, pid_t) -> Unmanaged
) -> CFRunLoopSource?
```

Deprecated

This functionality will be removed in a future release

## Parameters 

`sourceOrder`  

The order of the created run loop source.

`createMatchesCallback`  

A block to handle the font request.

## Return Value

A reference to a CFRunLoopSource object that should be added to the run loop. To stop receiving requests, invalidate this run loop source. Returns `NULL` on error, in the case of a duplicate `requestPortName`, or invalid context structure.

## See Also

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

func CTFontManagerCreateFontDescriptorFromData(CFData) -> CTFontDescriptor?

Creates a font descriptor representing the font in the supplied data.

func CTFontManagerCreateFontDescriptorsFromURL(CFURL) -> CFArray?

Returns an array of font descriptors representing each of the fonts in the specified URL.

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

