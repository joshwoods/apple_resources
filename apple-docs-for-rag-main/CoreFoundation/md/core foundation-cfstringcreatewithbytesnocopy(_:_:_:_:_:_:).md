

- Core Foundation
-  CFStringCreateWithBytesNoCopy(\_:\_:\_:\_:\_:\_:) 

Function

# CFStringCreateWithBytesNoCopy(\_:\_:\_:\_:\_:\_:)

Creates a string from a buffer, containing characters in a specified encoding, that might serve as the backing store for the new string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateWithBytesNoCopy(
    _ alloc: CFAllocator!,
    _ bytes: UnsafePointer!,
    _ numBytes: CFIndex,
    _ encoding: CFStringEncoding,
    _ isExternalRepresentation: Bool,
    _ contentsDeallocator: CFAllocator!
) -> CFString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFString object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

A buffer containing characters in the encoding specified by `encoding`. The buffer must *not* contain a length byte (as in Pascal buffers) or any terminating `NULL` character (as in C buffers).

`numBytes`  

The number of bytes in `bytes`.

`encoding`  

The character encoding of `bytes`.

`isExternalRepresentation`  

`true` if the characters in the byte buffer are in an “external representation” format—that is, whether the buffer contains a BOM (byte order marker). This is usually the case for bytes that are read in from a text file or received over the network. Otherwise, pass `false`.

`contentsDeallocator`  

The allocator to use to deallocate `bytes` when it is no longer needed. You can pass `NULL` or kCFAllocatorDefault to request the default allocator for this purpose. If the buffer does not need to be deallocated, or if you want to assume responsibility for deallocating the buffer (and not have the string deallocate it), pass kCFAllocatorNull.

## Return Value

A new string whose contents are `bytes`. Ownership follows the The Create Rule.

## Discussion

This function takes an explicit length, and allows you to specify whether the data is an external format—that is, whether to pay attention to the BOM character (if any) and do byte swapping if necessary

### Special Considerations

If an error occurs during the creation of the string, then `bytes` is not deallocated. In this case, the caller is responsible for freeing the buffer. This allows the caller to continue trying to create a string with the buffer, without having the buffer deallocated.

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

func CFStringCreateWithCharacters(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex) -> CFString!

Creates a string from a buffer of Unicode characters.

func CFStringCreateWithCharactersNoCopy(CFAllocator!, UnsafePointer&lt;UniChar>!, CFIndex, CFAllocator!) -> CFString!

Creates a string from a buffer of Unicode characters that might serve as the backing store for the object.

func CFStringCreateWithCString(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding) -> CFString!

Creates an immutable string from a C string.

func CFStringCreateWithCStringNoCopy(CFAllocator!, UnsafePointer&lt;CChar>!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external C string buffer that might serve as the backing store for the object.

func CFStringCreateWithFormatAndArguments(CFAllocator!, CFDictionary!, CFString!, CVaListPointer) -> CFString!

Creates an immutable string from a formatted string and a variable number of arguments (specified in a parameter of type `va_list`).

func CFStringCreateWithPascalString(CFAllocator!, ConstStr255Param!, CFStringEncoding) -> CFString!

Creates an immutable CFString object from a Pascal string.

func CFStringCreateWithPascalStringNoCopy(CFAllocator!, ConstStr255Param!, CFStringEncoding, CFAllocator!) -> CFString!

Creates a CFString object from an external Pascal string buffer that might serve as the backing store for the object.

func CFStringCreateWithSubstring(CFAllocator!, CFString!, CFRange) -> CFString!

Creates an immutable string from a segment (substring) of an existing string.

