

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  kUCTextBreakLeadingEdgeMask 

Global Variable

# kUCTextBreakLeadingEdgeMask

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCTextBreakLeadingEdgeMask: Int { get }
```

## Discussion

If the corresponding bit is set, then the starting offset for the `UCFindTextBreak` function is assumed to be in the word containing the character following the offset; this is the normal case when searching forward. If the corresponding bit is clear, then the starting offset for `UCFindTextBreak` is assumed to be in the word containing the character preceding the offset; this is the normal case when searching backward.

