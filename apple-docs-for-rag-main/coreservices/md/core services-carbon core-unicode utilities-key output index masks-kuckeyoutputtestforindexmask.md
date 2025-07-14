

- Core Services
- Carbon Core
- Unicode Utilities
- Key Output Index Masks
-  kUCKeyOutputTestForIndexMask 

Global Variable

# kUCKeyOutputTestForIndexMask

Mac Catalyst 13.0+macOS 10.0+

``` source
var kUCKeyOutputTestForIndexMask: Int { get }
```

## Discussion

You can use this mask to test the bits (14–15) in the `UCKeyOutput` value that determine whether the value contains an index to any other structure. If both bits specified by this mask are clear, the `UCKeyOutput` value does not contain an index to any other structure.

