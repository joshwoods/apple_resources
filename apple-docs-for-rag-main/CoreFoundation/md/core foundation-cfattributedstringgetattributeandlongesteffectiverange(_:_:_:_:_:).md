

- Core Foundation
-  CFAttributedStringGetAttributeAndLongestEffectiveRange(\_:\_:\_:\_:\_:) 

Function

# CFAttributedStringGetAttributeAndLongestEffectiveRange(\_:\_:\_:\_:\_:)

Returns the value of a given attribute of an attributed string at a specified location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringGetAttributeAndLongestEffectiveRange(
    _ aStr: CFAttributedString!,
    _ loc: CFIndex,
    _ attrName: CFString!,
    _ inRange: CFRange,
    _ longestEffectiveRange: UnsafeMutablePointer!
) -> CFTypeRef!
```

## Parameters 

`aStr`  

The attributed string to examine.

`loc`  

The location in `str` at which to determine the attributes. It is a programming error for `loc` to specify a location outside the bounds of `str`.

`attrName`  

The name of the attribute whose value you want to determine.

`inRange`  

The range in `str` within which you want to find the longest effective range of the attributes at `loc`. `inRange` must not exceed the bounds of `str`.

`longestEffectiveRange`  

If not `NULL`, upon return contains the maximal range within `inRange` over which the exact same set of attributes apply. The returned range is clipped to `inRange`.

## Return Value

A dictionary that contains the attributes of `str` at the specified location. Ownership follows the The Get Rule.

## See Also

### Accessing Attributes

func CFAttributedStringGetAttribute(CFAttributedString!, CFIndex, CFString!, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributes(CFAttributedString!, CFIndex, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

func CFAttributedStringGetAttributesAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

