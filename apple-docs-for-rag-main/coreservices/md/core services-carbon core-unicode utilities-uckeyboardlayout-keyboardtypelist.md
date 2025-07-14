

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyboardLayout
-  keyboardTypeList 

Instance Property

# keyboardTypeList

A variable-length array containing structures of type `UCKeyboardTypeHeader`. Each `UCKeyboardTypeHeader` entry specifies a range of physical keyboard types and contains offsets to each of the key mapping sections to be used for that range of keyboard types.

Mac Catalyst 13.0+macOS 10.0+

``` source
var keyboardTypeList: UCKeyboardTypeHeader
```

