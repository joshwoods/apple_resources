

- Core Services
- Carbon Core
- Unicode Utilities
-  UCTextBreakType 

Type Alias

# UCTextBreakType

Specifies kinds of text boundaries.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias UCTextBreakType = UInt32
```

## Topics

### Constants

var kUCTextBreakCharMask: Int

If the bit specified by this mask is set, boundaries of characters may be located (with surrogate pairs treated as a single character).

var kUCTextBreakClusterMask: Int

var kUCTextBreakWordMask: Int

If the bit specified by this mask is set, boundaries of words may be located. This can be used to determine what to highlight as the result of a double-click.

var kUCTextBreakLineMask: Int

If the bit specified by this mask is set, potential line breaks may be located.

