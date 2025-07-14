

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  kUCTextBreakIterateMask 

Global Variable

# kUCTextBreakIterateMask

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCTextBreakIterateMask: Int { get }
```

## Discussion

The corresponding bit may be set to indicate to the `UCFindTextBreak` function that the specified starting offset is a known break of the type specified in the `breakType` parameter. This permits `UCFindTextBreak` to optimize its search for the subsequent break of the same type. When iterating through all the breaks of a particular type in a particular buffer, this bit should be set for all calls except the first (since the initial `startOffset` value may not be a known break of the specified type).

