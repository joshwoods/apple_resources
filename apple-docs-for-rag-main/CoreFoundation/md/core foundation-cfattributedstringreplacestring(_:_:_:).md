

- Core Foundation
-  CFAttributedStringReplaceString(\_:\_:\_:) 

Function

# CFAttributedStringReplaceString(\_:\_:\_:)

Modifies the string of an attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringReplaceString(
    _ aStr: CFMutableAttributedString!,
    _ range: CFRange,
    _ replacement: CFString!
)
```

## Parameters 

`aStr`  

The mutable attributed string to modify.

`range`  

The range of `aStr` to be modified. `range` must not specify characters outside the bounds of `aStr`.

`replacement`  

The string to replace the existing string in `range`.

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

func CFAttributedStringReplaceAttributedString(CFMutableAttributedString!, CFRange, CFAttributedString!)

Replaces the attributed substring over a range with another attributed string.

func CFAttributedStringSetAttribute(CFMutableAttributedString!, CFRange, CFString!, CFTypeRef!)

Sets the value of a single attribute over the specified range.

func CFAttributedStringSetAttributes(CFMutableAttributedString!, CFRange, CFDictionary!, Bool)

Sets the value of attributes of a mutable attributed string over a specified range.

