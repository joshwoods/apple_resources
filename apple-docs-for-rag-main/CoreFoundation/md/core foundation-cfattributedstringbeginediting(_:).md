

- Core Foundation
-  CFAttributedStringBeginEditing(\_:) 

Function

# CFAttributedStringBeginEditing(\_:)

Defers internal consistency-checking and coalescing for a mutable attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringBeginEditing(_ aStr: CFMutableAttributedString!)
```

## Parameters 

`aStr`  

A mutable attributed string that is to be edited.

## Discussion

Defers internal consistency-checking and coalescing for a mutable attributed string. You must balance a call to this function with a corresponding CFAttributedStringEndEditing(_:).

## See Also

### Modifying a CFMutableAttributedString

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

func CFAttributedStringSetAttributes(CFMutableAttributedString!, CFRange, CFDictionary!, Bool)

Sets the value of attributes of a mutable attributed string over a specified range.

