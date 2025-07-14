

- Core Foundation
-  CFAttributedStringGetAttributes(\_:\_:\_:) 

Function

# CFAttributedStringGetAttributes(\_:\_:\_:)

Returns the attributes of an attributed string at a specified location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringGetAttributes(
    _ aStr: CFAttributedString!,
    _ loc: CFIndex,
    _ effectiveRange: UnsafeMutablePointer!
) -> CFDictionary!
```

## Parameters 

`aStr`  

The attributed string to examine.

`loc`  

The location in `str` at which to determine the attributes. `loc` must not exceed the bounds of `str`.

`effectiveRange`  

If not `NULL`, upon return contains a range including `loc` over which exactly the same set of attributes apply as at `loc`.

## Return Value

A dictionary that contains the attributes of `str` at the specified location. Ownership follows the The Get Rule.

## Discussion

For performance reasons, a range returned in `effectiveRange` is not necessarily the maximal range. If you need the maximum range, you should use CFAttributedStringGetAttributesAndLongestEffectiveRange(_:_:_:_:).

Note that the returned attribute dictionary might change in unpredictable ways if the attributed string is edited after this call. If you want to preserve the state of the dictionary, you should make an actual copy of it rather than just retaining it. In addition, you should make no assumptions about the relationship of the actual dictionary returned by this call and the dictionary originally used to set the attributes, other than the fact that the values stored in the dictionaries will be identical (that is, `==`) to those originally specified.

## See Also

### Accessing Attributes

func CFAttributedStringGetAttribute(CFAttributedString!, CFIndex, CFString!, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributeAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFString!, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributesAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

