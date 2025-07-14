

- Core Services
- Carbon Core
- Unicode Utilities
-  UCCollateOptions 

Type Alias

# UCCollateOptions

Specifies options for Unicode string comparison.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias UCCollateOptions = UInt32
```

## Discussion

For a description of the `UCCollateOptions` values, see Standard Options Mask.

## Topics

### Constants

var kUCCollateComposeInsensitiveMask: Int

var kUCCollateWidthInsensitiveMask: Int

var kUCCollateCaseInsensitiveMask: Int

If the corresponding bit is set, then uppercase and titlecase characters are treated as equivalent to the corresponding lowercase characters.

var kUCCollateDiacritInsensitiveMask: Int

If the corresponding bit is set, then characters with diacritics are treated as equivalent to the corresponding characters without diacritics.

var kUCCollatePunctuationSignificantMask: Int

var kUCCollateDigitsOverrideMask: Int

var kUCCollateDigitsAsNumberMask: Int

