

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  kUCCollatePunctuationSignificantMask 

Global Variable

# kUCCollatePunctuationSignificantMask

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCCollatePunctuationSignificantMask: Int { get }
```

## Discussion

If the corresponding bit is set, then punctuation and symbols are treated as significant instead of ignorable. This will produce results closer to the behavior of the older non-Unicode Mac OS collation functions. This option is available with Mac OS 9 and later.

