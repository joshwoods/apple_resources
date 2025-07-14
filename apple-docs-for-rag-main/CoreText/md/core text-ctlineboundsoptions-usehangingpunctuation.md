

- Core Text
- CTLineBoundsOptions
-  useHangingPunctuation 

Type Property

# useHangingPunctuation

An option to enable hanging punctuation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var useHangingPunctuation: CTLineBoundsOptions { get }
```

## Discussion

The result of this option moves standard punctuation, such as periods, commas, hyphens, dashes, quotation marks, and asterisks, into the margin of either end of text, to give the appearance of a more uniform vertical alignment. Consider using this option when the text is fully justified.

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

static var useOpticalBounds: CTLineBoundsOptions

An option to use optical bounds.

