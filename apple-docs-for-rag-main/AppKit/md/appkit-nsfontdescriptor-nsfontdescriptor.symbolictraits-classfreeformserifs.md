

- AppKit
- NSFontDescriptor
- NSFontDescriptor.SymbolicTraits
-  classFreeformSerifs 

Type Property

# classFreeformSerifs

The font’s characters include serifs, and don’t generally fit within other serif design classifications.

macOS

``` source
static var classFreeformSerifs: NSFontDescriptor.SymbolicTraits { get }
```

## See Also

### Symbolic Traits

static var italic: NSFontDescriptor.SymbolicTraits

The font’s style is italic.

static var bold: NSFontDescriptor.SymbolicTraits

The font’s style is boldface.

static var expanded: NSFontDescriptor.SymbolicTraits

The font’s characters have an expanded width.

static var condensed: NSFontDescriptor.SymbolicTraits

The font’s characters have a condensed width.

static var monoSpace: NSFontDescriptor.SymbolicTraits

The font’s characters all have the same width.

static var vertical: NSFontDescriptor.SymbolicTraits

The font uses vertical glyph variants and metrics.

static var UIOptimized: NSFontDescriptor.SymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as in control titles, if necessary.

static var tightLeading: NSFontDescriptor.SymbolicTraits

The font uses a leading value that’s less than the default.

static var looseLeading: NSFontDescriptor.SymbolicTraits

The font uses a leading value that’s greater than the default.

static var classMask: NSFontDescriptor.SymbolicTraits

The font family class mask that you use to access font descriptor values.

static var classOldStyleSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 15th to 17th centuries.

static var classTransitionalSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 18th to 19th centuries.

static var classModernSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include serifs, and reflect the Latin printing style of the 20th century.

static var classClarendonSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters include variations of old style and transitional serifs.

static var classSlabSerifs: NSFontDescriptor.SymbolicTraits

The font’s characters use square transitions, without brackets, between strokes and serifs.

