

- Core Text
-  CTFontManagerUnregisterFontURLs(\_:\_:\_:) 

Function

# CTFontManagerUnregisterFontURLs(\_:\_:\_:)

Unregisters fonts from the specified font URLs with the font manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func CTFontManagerUnregisterFontURLs(
    _ fontURLs: CFArray,
    _ scope: CTFontManagerScope,
    _ registrationHandler: ((CFArray, Bool) -> Bool)?
)
```

## Parameters 

`fontURLs`  

An array of font URLs.

`scope`  

A scope constant that defines the availability and lifetime of the registration. This value should match the scope the fonts are registered in. See CTFontManagerScope for more details.

`registrationHandler`  

A block called as errors arise or upon completion.

The block’s `errors` parameter contains an array of CFError references; an empty array indicates no errors unregistering the files. Each error reference contains a CFArray of font URLs corresponding to kCTFontManagerErrorFontURLsKey. These URLs represent the font files causing the error and failing to unregister successfully.

This block may be called multiple times during the unregistration process. The `done` parameter becomes true when the unregistration process completes. Return false from the block to stop the unregistration operation, like after receiving an error.

## Discussion

Unregistered fonts don’t participate in font descriptor matching.

Note

On iOS, you can only use this function to unregister fonts that you registered using CTFontManagerRegisterFontsForURL(_:_:_:) or CTFontManagerRegisterFontsForURLs(_:_:_:).

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

