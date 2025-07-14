

- Core Text
- CTFontSymbolicTraits
-  traitMonoSpace 

Type Property

# traitMonoSpace

The font uses fixed-pitch glyphs if available.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var traitMonoSpace: CTFontSymbolicTraits { get }
```

## Discussion

The font may have multiple glyph advances (many CJK glyphs contain two spaces).

## See Also

### Symbolic Traits

static var traitItalic: CTFontSymbolicTraits

The font typestyle is italic.

static var traitBold: CTFontSymbolicTraits

The font typestyle is boldface.

static var traitExpanded: CTFontSymbolicTraits

The font typestyle is expanded.

static var traitCondensed: CTFontSymbolicTraits

The font typestyle is condensed.

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

