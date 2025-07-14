

- Core Services
- Carbon Core
- Unicode Utilities
- Standard Options Mask
-  kUCCollateStandardOptions 

Global Variable

# kUCCollateStandardOptions

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCCollateStandardOptions: Int { get }
```

## Discussion

If the `kUCCollateComposeInsensitiveMask` and `kUCCollateWidthInsensitiveMask` bits are set, then (1) precomposed and decomposed representations of the same text element will be treated as equivalent, and (2) fullwidth and halfwidth compatibility forms will be treated as equivalent to the corresponding non-compatibility characters.

