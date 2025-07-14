

- Core Foundation
-  CFAttributedStringReplaceAttributedString(\_:\_:\_:) 

Function

# CFAttributedStringReplaceAttributedString(\_:\_:\_:)

Replaces the attributed substring over a range with another attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringReplaceAttributedString(
    _ aStr: CFMutableAttributedString!,
    _ range: CFRange,
    _ replacement: CFAttributedString!
)
```

## Parameters 

`aStr`  

The mutable attributed string to modify.

`range`  

The range of `aStr` to be modified. `range` must not specify characters outside the bounds of `aStr`.

`replacement`  

The attributed string to replace the contents of `aStr` in `range`.

## See Also

### Modifying a CFMutableAttributedString

func CFAttributedStringBeginEditing(CFMutableAttributedString!)

Defers internal consistency-checking and coalescing for a mutable attributed string.

func CFAttributedStringEndEditing(CFMutableAttributedString!)

Re-enables internal consistency-checking and coalescing for a mutable attributed string.

func CFAttributedStringGetMutableString(CFMutableAttributedString!) -> CFMutableString!

Gets as a mutable string the string for an attributed string.

func CFAttributedStringRemoveAttribute(CFMutableAttributedString!, CFRange, CFString!)

Removes the value of a single attribute over a specified range.

func CFAttributedStringReplaceString(CFMutableAttributedString!, CFRange, CFString!)

Modifies the string of an attributed string.

func CFAttributedStringSetAttribute(CFMutableAttributedString!, CFRange, CFString!, CFTypeRef!)

Sets the value of a single attribute over the specified range.

func CFAttributedStringSetAttributes(CFMutableAttributedString!, CFRange, CFDictionary!, Bool)

Sets the value of attributes of a mutable attributed string over a specified range.

