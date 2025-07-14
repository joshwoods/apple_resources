

- Core Services
- Carbon Core
- Unicode Utilities
-  UCCollationValue 

Type Alias

# UCCollationValue

Specifies a Unicode collation key.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias UCCollationValue = UInt32
```

## Discussion

Collation keys consist of an array of `UCCollationValue` values. The collation key consists of a sequence of primary weights for all of the collation text elements in the string, followed by a separator and a sequence of secondary weights for all of the text elements in the string, and so on for several levels of significance. The separator is usually 0; however, 1 is used as the separator at the boundary between levels that are significant and levels that are insignificant for the options you supply in the collator object. You can obtain a collation key with the function UCGetCollationKey(_:_:_:_:_:_:).

