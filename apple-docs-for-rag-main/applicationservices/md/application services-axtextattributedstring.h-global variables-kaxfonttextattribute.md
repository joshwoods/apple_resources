

- Application Services
- AXTextAttributedString.h
- Global Variables
-  kAXFontTextAttribute 

Global Variable

# kAXFontTextAttribute

A dictionary (a `CFDictionaryRef`) of two or more font keys.

macOS 10.4+

``` source
var kAXFontTextAttribute: Unmanaged
```

## Discussion

The dictionary associated with this attribute must contain the kAXFontNameKey and kAXFontSizeKey font keys. It may also contain the kAXFontFamilyKey and kAXVisibleNameKey font keys.

