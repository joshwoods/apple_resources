

- Core Foundation
-  CFAttributedStringSetAttribute(\_:\_:\_:\_:) 

Function

# CFAttributedStringSetAttribute(\_:\_:\_:\_:)

Sets the value of a single attribute over the specified range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringSetAttribute(
    _ aStr: CFMutableAttributedString!,
    _ range: CFRange,
    _ attrName: CFString!,
    _ value: CFTypeRef!
)
```

## Parameters 

`aStr`  

The mutable attributed string to modify.

`range`  

The range of `aStr` over to which the new attributes apply. `range` must not exceed the bounds of `aStr`.

`attrName`  

The name of the attribute whose value to set.

`value`  

The value of the attribute `attrName` to apply over `range`. This value may not be `NULL`. If you want to remove an attribute, use CFAttributedStringRemoveAttribute(_:_:_:).

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

func CFAttributedStringReplaceAttributedString(CFMutableAttributedString!, CFRange, CFAttributedString!)

Replaces the attributed substring over a range with another attributed string.

func CFAttributedStringSetAttributes(CFMutableAttributedString!, CFRange, CFDictionary!, Bool)

Sets the value of attributes of a mutable attributed string over a specified range.

