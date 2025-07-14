

- Core Foundation
-  CFStringCreateWithFormatAndArguments(\_:\_:\_:\_:) 

Function

# CFStringCreateWithFormatAndArguments(\_:\_:\_:\_:)

Creates an immutable string from a formatted string and a variable number of arguments (specified in a parameter of type `va_list`).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateWithFormatAndArguments(
    _ alloc: CFAllocator!,
    _ formatOptions: CFDictionary!,
    _ format: CFString!,
    _ arguments: CVaListPointer
) -> CFString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatOptions`  

A CFDictionary object containing formatting options for the string (such as the thousand-separator character, which is dependent on locale). Currently, these options are an unimplemented feature.

`format`  

The formatted string with `printf`-style specifiers. For information on supported specifiers, see String Format Specifiers.

`arguments`  

The variable argument list of values to be inserted into the formatted string contained in `format`.

## Return Value

An immutable string, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

The programming interface for variable argument lists (`va_list`, `va_start`, `va_end`, and so forth) is declared in the standard C header file `stdarg.h`.

## See Also

### Creating a CFString

func CFStringCreateArrayBySeparatingStrings(CFAllocator!, CFString!, CFString!) -> CFArray!

Creates an array of CFString objects from a single CFString object.

func CFStringCreateByCombiningStrings(CFAllocator!, CFArray!, CFString!) -> CFString!

Creates a single string from the individual CFString objects that comprise the elements of an array.

func CFStringCreateCopy(CFAllocator!, CFString!) -> CFString!

Creates an immutable copy of a string.

func CFStringCreateFromExternalRepresentation(CFAllocator!, CFData!, CFStringEncoding) -> CFString!

Creates a string from its “external representation.”

func CFStringCreateWithBytes(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, Bool) -> CFString!

Creates a string from a buffer containing characters in a specified encoding.

func CFStringCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFStringEncoding, Bool, CFAllocator!) -> CFString!

Creates a string from a buffer, containing characters in a specified encoding, that might serve as the backing store for the new string.

func CFStringCreateWithCharacters(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex) -> CFString!

Creates a string from a buffer of Unicode characters.

func CFStringCreateWithCharactersNoCopy(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex, CFAllocator!) -> CFString!

Creates a string from a buffer of Unicode characters that might serve as the backing store for the object.

func CFStringCreateWithCString(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding) -> CFString!

Creates an immutable string from a C string.

func CFStringCreateWithCStringNoCopy(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external C string buffer that might serve as the backing store for the object.

func CFStringCreateWithPascalString(CFAllocator!, ConstStr255Param!, CFStringEncoding) -> CFString!

Creates an immutable CFString object from a Pascal string.

func CFStringCreateWithPascalStringNoCopy(CFAllocator!, ConstStr255Param!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external Pascal string buffer that might serve as the backing store for the object.

func CFStringCreateWithSubstring(CFAllocator!, CFString!, CFRange) -> CFString!

Creates an immutable string from a segment (substring) of an existing string.

