

- Core Foundation
-  CFAttributedStringGetAttribute(\_:\_:\_:\_:) 

Function

# CFAttributedStringGetAttribute(\_:\_:\_:\_:)

Returns the value of a given attribute of an attributed string at a specified location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringGetAttribute(
    _ aStr: CFAttributedString!,
    _ loc: CFIndex,
    _ attrName: CFString!,
    _ effectiveRange: UnsafeMutablePointer!
) -> CFTypeRef!
```

## Parameters 

`aStr`  

The attributed string to examine.

`loc`  

The location in `str` at which to determine the attributes. `loc` must not exceed the bounds of `str`.

`attrName`  

The name of the attribute whose value you want to determine.

`effectiveRange`  

If not `NULL`, upon return contains a range including `loc` over which exactly the same set of attributes apply as at `loc`.

## Return Value

The value of the specified attribute at the specified location in `str`. Ownership follows the The Get Rule.

## Discussion

For performance reasons, a range returned in `effectiveRange` is not necessarily the maximal range. If you need the maximum range, you should use CFAttributedStringGetAttributeAndLongestEffectiveRange(_:_:_:_:_:).

## See Also

### Accessing Attributes

func CFAttributedStringGetAttributes(CFAttributedString!, CFIndex, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

func CFAttributedStringGetAttributeAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFString!, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributesAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

