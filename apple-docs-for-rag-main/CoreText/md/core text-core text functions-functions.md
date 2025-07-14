

- Core Text
-  Core Text Functions 

API Collection

# Core Text Functions

## Topics

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

func CTFontManagerSetAutoActivationSetting(CFString?, CTFontManagerAutoActivationSetting)

Sets the auto-activation setting for the specified bundle identifier.

func CTFontManagerUnregisterFontsForURL(CFURL, CTFontManagerScope, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Unregisters fonts from the specified font URL with the Font Manager. Unregistered fonts are no longer discoverable through font descriptor matching.

func CTFontManagerUnregisterFontsForURLs(CFArray, CTFontManagerScope, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>?) -> Bool

Unregisters fonts from the specified array of font URLs with the Font Manager. Unregistered fonts are no longer discoverable through font descriptor matching.

Deprecated

func CTFontManagerUnregisterGraphicsFont(CGFont, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Unregisters the specified graphics font with the font manager.

Deprecated

func CTFontManagerCopyRegisteredFontDescriptors(CTFontManagerScope, Bool) -> CFArray

Retrieves the font descriptors that were registered with the font manager.

func CTFontManagerCreateFontDescriptorsFromData(CFData) -> CFArray

Creates an array of font descriptors for the fonts in the supplied data.

func CTFontManagerRegisterFontDescriptors(CFArray, CTFontManagerScope, Bool, ((CFArray, Bool) -> Bool)?)

Registers font descriptors with the font manager.

func CTFontManagerRegisterFontURLs(CFArray, CTFontManagerScope, Bool, ((CFArray, Bool) -> Bool)?)

Registers fonts from the specified font URLs with the font manager.

func CTFontManagerRegisterFontsWithAssetNames(CFArray, CFBundle?, CTFontManagerScope, Bool, ((CFArray, Bool) -> Bool)?)

Registers named font assets in the specified bundle with the font manager.

func CTFontManagerRequestFonts(CFArray, (CFArray) -> Void)

Resolves font descriptors specified on input.

func CTFontManagerUnregisterFontDescriptors(CFArray, CTFontManagerScope, ((CFArray, Bool) -> Bool)?)

Unregisters font descriptors with the font manager.

func CTFontManagerUnregisterFontURLs(CFArray, CTFontManagerScope, ((CFArray, Bool) -> Bool)?)

Unregisters fonts from the specified font URLs with the font manager.

func CTGetCoreTextVersion() -> UInt32

Returns the version of the Core Text framework.

Deprecated

func CTRubyAnnotationCreate(CTRubyAlignment, CTRubyOverhang, CGFloat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> CTRubyAnnotation

Creates an immutable ruby annotation object.

func CTRubyAnnotationCreateCopy(CTRubyAnnotation) -> CTRubyAnnotation

Creates an immutable copy of a ruby annotation object.

func CTRubyAnnotationCreateWithAttributes(CTRubyAlignment, CTRubyOverhang, CTRubyPosition, CFString, CFDictionary) -> CTRubyAnnotation

Creates an immutable ruby annotation object with the specified attributes.

func CTRubyAnnotationGetAlignment(CTRubyAnnotation) -> CTRubyAlignment

Retrieves the alignment value of a ruby annotation object.

func CTRubyAnnotationGetOverhang(CTRubyAnnotation) -> CTRubyOverhang

Retrieves the overhang value of a ruby annotation object.

func CTRubyAnnotationGetSizeFactor(CTRubyAnnotation) -> CGFloat

Retrieves the size factor of a ruby annotation object.

func CTRubyAnnotationGetTextForPosition(CTRubyAnnotation, CTRubyPosition) -> CFString?

Retrieves the ruby text for a particular position in a ruby annotation.

func CTRubyAnnotationGetTypeID() -> CFTypeID

Retrieves the type of the ruby annotation object.

func CTFontCopyNameForGlyph(CTFont, CGGlyph) -> CFString?

Retrieves the name for the specified glyph.

func CTFontDrawImageFromAdaptiveImageProviderAtPoint(CTFont, any CTAdaptiveImageProviding, CGPoint, CGContext)

func CTFontGetTypographicBoundsForAdaptiveImageProvider(CTFont, (any CTAdaptiveImageProviding)?) -> CGRect

func CTFontHasTable(CTFont, CTFontTableTag) -> Bool

## See Also

### Reference

Styling Attributed Strings

Attributes to which Core Text responds when placed in a `CFAttributedString` object.

Core Text Structures

Core Text Enumerations

Core Text Constants

Core Text Data Types

SFNT Support

