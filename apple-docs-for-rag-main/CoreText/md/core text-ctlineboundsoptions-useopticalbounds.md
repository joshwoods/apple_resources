

- Core Text
- CTLineBoundsOptions
-  useOpticalBounds 

Type Property

# useOpticalBounds

An option to use optical bounds.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var useOpticalBounds: CTLineBoundsOptions { get }
```

## Discussion

This option overrides useGlyphPathBounds.

## See Also

### Line Bounds Options

static var excludeTypographicLeading: CTLineBoundsOptions

An option to exclude typographic leading.

static var excludeTypographicShifts: CTLineBoundsOptions

An option to ignore cross-stream shifts due to positioning, such as kerning or baseline alignment.

static var includeLanguageExtents: CTLineBoundsOptions

An option to include additional space based on common glyph sequences for various languages.

static var useGlyphPathBounds: CTLineBoundsOptions

An option to use glyph path bounds rather than the default typographic bounds.

static var useHangingPunctuation: CTLineBoundsOptions

An option to enable hanging punctuation.

