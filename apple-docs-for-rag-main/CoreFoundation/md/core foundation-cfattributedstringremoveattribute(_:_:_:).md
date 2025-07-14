

- Core Foundation
-  CFAttributedStringRemoveAttribute(\_:\_:\_:) 

Function

# CFAttributedStringRemoveAttribute(\_:\_:\_:)

Removes the value of a single attribute over a specified range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringRemoveAttribute(
    _ aStr: CFMutableAttributedString!,
    _ range: CFRange,
    _ attrName: CFString!
)
```

## Parameters 

`aStr`  

The mutable attributed string to modify.

`range`  

The range of `aStr` from which to remove the specified attribute. `range` must not exceed the bounds of `aStr`.

`attrName`  

The name of the attribute to remove.

## Discussion

It is *not* an error of the specified attribute does not exist over the given range.

## See Also

### Modifying a CFMutableAttributedString

func CFAttributedStringBeginEditing(CFMutableAttributedString!)

Defers internal consistency-checking and coalescing for a mutable attributed string.

func CFAttributedStringEndEditing(CFMutableAttributedString!)

Re-enables internal consistency-checking and coalescing for a mutable attributed string.

func CFAttributedStringGetMutableString(CFMutableAttributedString!) -> CFMutableString!

Gets as a mutable string the string for an attributed string.

func CFAttributedStringReplaceString(CFMutableAttributedString!, CFRange, CFString!)

Modifies the string of an attributed string.

func CFAttributedStringReplaceAttributedString(CFMutableAttributedString!, CFRange, CFAttributedString!)

Replaces the attributed substring over a range with another attributed string.

func CFAttributedStringSetAttribute(CFMutableAttributedString!, CFRange, CFString!, CFTypeRef!)

Sets the value of a single attribute over the specified range.

func CFAttributedStringSetAttributes(CFMutableAttributedString!, CFRange, CFDictionary!, Bool)

Sets the value of attributes of a mutable attributed string over a specified range.

