

- Core Text
-  CTFontManagerRegisterFontsWithAssetNames(\_:\_:\_:\_:\_:) 

Function

# CTFontManagerRegisterFontsWithAssetNames(\_:\_:\_:\_:\_:)

Registers named font assets in the specified bundle with the font manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func CTFontManagerRegisterFontsWithAssetNames(
    _ fontAssetNames: CFArray,
    _ bundle: CFBundle?,
    _ scope: CTFontManagerScope,
    _ enabled: Bool,
    _ registrationHandler: ((CFArray, Bool) -> Bool)?
)
```

## Parameters 

`fontAssetNames`  

An array of font name assets in the asset catalog.

`bundle`  

A bundle that contains the asset catalog. Passing `NULL` resolves to the main bundle.

`scope`  

A scope constant that defines the availability and lifetime of the registration. On iOS, the only supported scope is CTFontManagerScope.persistent, which means the fonts aren’t automatically available to other processes. Other processes can call CTFontManagerRequestFonts(_:_:) to get access to the fonts. See CTFontManagerScope for more details.

`enabled`  

A Boolean value that indicates whether the font assets should be enabled for font descriptor matching and discoverable through CTFontManagerRequestFonts(_:_:).

`registrationHandler`  

A block called as errors arise or upon completion.

The block’s `errors` parameter contains an array of CFError references; an empty array indicates no errors. Each error reference contains a CFArray of font asset names corresponding to kCTFontManagerErrorFontAssetNameKey. These represent the font asset names causing the error and failing to register successfully.

This block may be called multiple times during the registration process. The `done` parameter becomes true when the registration process completes. Return false from the block to stop the registration operation, like after receiving an error.

## Discussion

Registered fonts are discoverable through font descriptor matching in the calling process.

Calling this function extracts the font assets from the asset catalog and registers them. You must make this call after the completion handler of either beginAccessingResources(completionHandler:): or conditionallyBeginAccessingResources(completionHandler:) is called successfully.

Name the assets using PostScript names for individual faces, or family names for variable or collection fonts. You can use the same names to unregister the fonts with CTFontManagerUnregisterFontDescriptors(_:_:_:).

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

