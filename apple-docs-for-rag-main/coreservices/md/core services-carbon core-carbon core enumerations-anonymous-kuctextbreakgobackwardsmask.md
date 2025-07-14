

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  kUCTextBreakGoBackwardsMask 

Global Variable

# kUCTextBreakGoBackwardsMask

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCTextBreakGoBackwardsMask: Int { get }
```

## Discussion

If the corresponding bit is set, then `UCFindTextBreak` searches backward from the value provided in its `startOffset` parameter to find the next text break. If the corresponding bit is clear, then `UCFindTextBreak` searches forward from the `startOffset` value to find the next text break.

