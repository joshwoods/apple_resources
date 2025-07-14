

- Core Foundation
-  CFAttributedStringSetAttributes(\_:\_:\_:\_:) 

Function

# CFAttributedStringSetAttributes(\_:\_:\_:\_:)

Sets the value of attributes of a mutable attributed string over a specified range.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringSetAttributes(
    _ aStr: CFMutableAttributedString!,
    _ range: CFRange,
    _ replacement: CFDictionary!,
    _ clearOtherAttributes: Bool
)
```

## Parameters 

`aStr`  

The mutable attributed string to modify.

`range`  

The range of aStr over to which the new attributes apply. `range` must not exceed the bounds of `aStr`.

`replacement`  

A dictionary that contains key-value pairs that specify the new attributes to apply to `range`. The keys must be CFString objects, and the corresponding values must be CFType objects.

`clearOtherAttributes`  

If `false`, existing attributes (that aren’t being replaced) are left alone; otherwise they are cleared.

## Discussion

Note that after this call, if it is mutable, changes to `replacement` will not affect the contents of the attributed string.

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

func CFAttributedStringSetAttribute(CFMutableAttributedString!, CFRange, CFString!, CFTypeRef!)

Sets the value of a single attribute over the specified range.

