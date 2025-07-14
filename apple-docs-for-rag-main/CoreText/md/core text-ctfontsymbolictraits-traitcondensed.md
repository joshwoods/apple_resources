

- Core Text
- CTFontSymbolicTraits
-  traitCondensed 

Type Property

# traitCondensed

The font typestyle is condensed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var traitCondensed: CTFontSymbolicTraits { get }
```

## Discussion

Additional detail is available via kCTFontWidthTrait.

Important

expandedTrait and condensedTrait are mutually exclusive.

## See Also

### Related Documentation

let kCTFontWidthTrait: CFString

The normalized proportion (width condense or expand) trait from the font traits dictionary.

### Symbolic Traits

static var traitItalic: CTFontSymbolicTraits

The font typestyle is italic.

static var traitBold: CTFontSymbolicTraits

The font typestyle is boldface.

static var traitExpanded: CTFontSymbolicTraits

The font typestyle is expanded.

static var traitMonoSpace: CTFontSymbolicTraits

The font uses fixed-pitch glyphs if available.

static var traitVertical: CTFontSymbolicTraits

The font uses vertical glyph variants and metrics.

static var traitUIOptimized: CTFontSymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as control titles, if necessary.

static var traitColorGlyphs: CTFontSymbolicTraits

The font contains color glyphs.

static var traitComposite: CTFontSymbolicTraits

The font is in Composite Font Reference format.

static var traitClassMask: CTFontSymbolicTraits

Mask for the font class.

