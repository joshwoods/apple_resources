

- Core Foundation
-  CFAttributedStringGetLength(\_:) 

Function

# CFAttributedStringGetLength(\_:)

Returns the length of the attributed string in characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAttributedStringGetLength(_ aStr: CFAttributedString!) -> CFIndex
```

## Parameters 

`aStr`  

The attributed string to examine.

## Return Value

The length of the attributed string in characters; this is the same as `CFStringGetLength(CFAttributedStringGetString(aStr))`.

## See Also

### Creating a CFAttributedString

func CFAttributedStringCreate(CFAllocator!, CFString!, CFDictionary!) -> CFAttributedString!

Creates an attributed string with specified string and attributes.

func CFAttributedStringCreateCopy(CFAllocator!, CFAttributedString!) -> CFAttributedString!

Creates an immutable copy of an attributed string.

func CFAttributedStringCreateWithSubstring(CFAllocator!, CFAttributedString!, CFRange) -> CFAttributedString!

Creates a sub-attributed string from the specified range.

func CFAttributedStringGetString(CFAttributedString!) -> CFString!

Returns the string for an attributed string.

