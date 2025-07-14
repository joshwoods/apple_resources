

- Core Text
- CTFontSymbolicTraits
-  traitComposite 

Type Property

# traitComposite

The font is in Composite Font Reference format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var traitComposite: CTFontSymbolicTraits { get }
```

## Discussion

For CFR, a cascade list is expected per font.

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

static var traitMonoSpace: CTFontSymbolicTraits

The font uses fixed-pitch glyphs if available.

static var traitVertical: CTFontSymbolicTraits

The font uses vertical glyph variants and metrics.

static var traitUIOptimized: CTFontSymbolicTraits

The font synthesizes appropriate attributes for user interface rendering, such as control titles, if necessary.

static var traitColorGlyphs: CTFontSymbolicTraits

The font contains color glyphs.

static var traitClassMask: CTFontSymbolicTraits

Mask for the font class.

