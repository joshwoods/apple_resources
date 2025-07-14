

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyboardTypeHeader
-  keyboardTypeFirst 

Instance Property

# keyboardTypeFirst

An unsigned 32-bit integer specifying the first keyboard type in this entry. For the initial entry (that is, the default entry) in an array of `UCKeyboardTypeHeader` structures, you should set this value to 0. The initial `UCKeyboardTypeHeader` entry is used if the keyboard type passed to the function UCKeyTranslate(_:_:_:_:_:_:_:_:_:_:) does not match any other entry, that is, if it is not within the range of values specified by `keyboardTypeFirst` and `keyboardTypeLast` for any entry.

Mac Catalyst 13.0+macOS 10.0+

``` source
var keyboardTypeFirst: UInt32
```

