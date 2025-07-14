

- Core Text
- CTLineBoundsOptions
-  includeLanguageExtents 

Type Property

# includeLanguageExtents

An option to include additional space based on common glyph sequences for various languages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var includeLanguageExtents: CTLineBoundsOptions { get }
```

## Discussion

Use the result of this option when drawing to avoid clipping that the typographic bounds may cause. This option doesn’t have an effect when you use it with useGlyphPathBounds.

## See Also

### Line Bounds Options

static var excludeTypographicLeading: CTLineBoundsOptions

An option to exclude typographic leading.

static var excludeTypographicShifts: CTLineBoundsOptions

An option to ignore cross-stream shifts due to positioning, such as kerning or baseline alignment.

static var useGlyphPathBounds: CTLineBoundsOptions

An option to use glyph path bounds rather than the default typographic bounds.

static var useHangingPunctuation: CTLineBoundsOptions

An option to enable hanging punctuation.

static var useOpticalBounds: CTLineBoundsOptions

An option to use optical bounds.

