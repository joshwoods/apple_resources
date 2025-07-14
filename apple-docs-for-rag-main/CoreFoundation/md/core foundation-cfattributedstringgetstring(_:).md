

- Core Foundation
-  CFAttributedStringGetString(\_:) 

Function

# CFAttributedStringGetString(\_:)

Returns the string for an attributed string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringGetString(_ aStr: CFAttributedString!) -> CFString!
```

## Parameters 

`aStr`  

The attributed string to examine.

## Return Value

An immutable string containing the characters from `aStr`, or `NULL` if there was a problem creating the object. Ownership follows the The Get Rule.

## Discussion

For performance reasons, the string returned will often be the backing store of the attributed string, and it might therefore change if the attributed string is edited. However, this is an implementation detail, and you should not rely on this behavior.

## See Also

### Creating a CFAttributedString

func CFAttributedStringCreate(CFAllocator!, CFString!, CFDictionary!) -> CFAttributedString!

Creates an attributed string with specified string and attributes.

func CFAttributedStringCreateCopy(CFAllocator!, CFAttributedString!) -> CFAttributedString!

Creates an immutable copy of an attributed string.

func CFAttributedStringCreateWithSubstring(CFAllocator!, CFAttributedString!, CFRange) -> CFAttributedString!

Creates a sub-attributed string from the specified range.

func CFAttributedStringGetLength(CFAttributedString!) -> CFIndex

Returns the length of the attributed string in characters.

