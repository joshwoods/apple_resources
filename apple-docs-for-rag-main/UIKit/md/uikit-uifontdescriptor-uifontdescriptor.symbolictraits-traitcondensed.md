

- UIKit
- UIFontDescriptor
- UIFontDescriptor.SymbolicTraits
-  traitCondensed 

Type Property

# traitCondensed

The font’s characters have a condensed width.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
static var traitCondensed: UIFontDescriptor.SymbolicTraits { get }
```

## Discussion

Expanded and condensed traits are mutually exclusive.

## See Also

### Font traits

static var traitItalic: UIFontDescriptor.SymbolicTraits

The font’s style is italic.

static var traitBold: UIFontDescriptor.SymbolicTraits

The font’s style is boldface.

static var traitExpanded: UIFontDescriptor.SymbolicTraits

The font’s characters have an expanded width.

static var traitMonoSpace: UIFontDescriptor.SymbolicTraits

The font’s characters all have the same width.

static var traitVertical: UIFontDescriptor.SymbolicTraits

The font uses vertical glyph variants and metrics.

static var traitUIOptimized: UIFontDescriptor.SymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as in control titles, if necessary.

static var traitTightLeading: UIFontDescriptor.SymbolicTraits

The font uses a leading value that’s less than the default.

static var traitLooseLeading: UIFontDescriptor.SymbolicTraits

The font uses a leading value that’s greater than the default.

static var classMask: UIFontDescriptor.SymbolicTraits

The font family class mask that you use to access font descriptor values.

static var classOldStyleSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 15th to 17th centuries.

static var classTransitionalSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 18th to 19th centuries.

static var classModernSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 20th century.

static var classClarendonSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include variations of old style and transitional serifs.

static var classSlabSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters use square transitions, without brackets, between strokes and serifs.

static var classFreeformSerifs: UIFontDescriptor.SymbolicTraits

The font’s characters include serifs, and don’t generally fit within other serif design classifications.

