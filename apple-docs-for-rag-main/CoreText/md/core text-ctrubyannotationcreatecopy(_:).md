

- Core Text
-  CTRubyAnnotationCreateCopy(\_:) 

Function

# CTRubyAnnotationCreateCopy(\_:)

Creates an immutable copy of a ruby annotation object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRubyAnnotationCreateCopy(_ rubyAnnotation: CTRubyAnnotation) -> CTRubyAnnotation
```

## Parameters 

`rubyAnnotation`  

The ruby annotation object to copy.

## Return Value

A valid reference to an immutable CTRubyAnnotation object that’s a copy of `rubyAnnotation`, if the `rubyAnnotation` object is valid.

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

