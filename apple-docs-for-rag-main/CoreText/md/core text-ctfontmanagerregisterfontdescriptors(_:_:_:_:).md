

- Core Text
-  CTFontManagerRegisterFontDescriptors(\_:\_:\_:\_:) 

Function

# CTFontManagerRegisterFontDescriptors(\_:\_:\_:\_:)

Registers font descriptors with the font manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func CTFontManagerRegisterFontDescriptors(
    _ fontDescriptors: CFArray,
    _ scope: CTFontManagerScope,
    _ enabled: Bool,
    _ registrationHandler: ((CFArray, Bool) -> Bool)?
)
```

## Parameters 

`fontDescriptors`  

An array of font descriptors to register. The font descriptor keys for registration are kCTFontURLAttribute, kCTFontNameAttribute, kCTFontFamilyNameAttribute, or kCTFontRegistrationUserInfoAttribute.

`scope`  

A scope constant that defines the availability and lifetime of the registration. If you specify CTFontManagerScope.persistent when you register fonts on iOS, those fonts aren’t automatically available to other processes. Other processes can call CTFontManagerRequestFonts(_:_:) to get access to those fonts. See CTFontManagerScope for more details.

`enabled`  

A Boolean value that indicates whether the font descriptors should be enabled for font descriptor matching and discoverable though CTFontManagerRequestFonts(_:_:).

`registrationHandler`  

A block called as errors arise or upon completion.

The block’s `errors` parameter contains an array of CFError references; an empty array indicates no errors. Each error reference contains a CFArray of font descriptors corresponding to kCTFontManagerErrorFontDescriptorsKey. These represent the font descriptors causing the error and failing to register successfully.

This block may be called multiple times during the registration process. The `done` parameter becomes true when the registration process completes. Return false from the block to stop the registration operation, like after receiving an error.

## Discussion

Registered fonts are discoverable through font descriptor matching in the calling process.

Fonts descriptors registered in a disabled state (the `enabled` parameter set to false) aren’t immediately available for descriptor matching, but the font manager knows the descriptors can be made available if necessary. You can enable these descriptors by calling this function again with the `enabled` parameter set to true. This operation may fail if there’s another registered and enabled font with the same PostScript name.

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

