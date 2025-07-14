

- Core Foundation
-  CFStringCreateMutableWithExternalCharactersNoCopy(\_:\_:\_:\_:\_:) 

Function

# CFStringCreateMutableWithExternalCharactersNoCopy(\_:\_:\_:\_:\_:)

Creates a CFMutableString object whose Unicode character buffer is controlled externally.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateMutableWithExternalCharactersNoCopy(
    _ alloc: CFAllocator!,
    _ chars: UnsafeMutablePointer!,
    _ numChars: CFIndex,
    _ capacity: CFIndex,
    _ externalCharactersAllocator: CFAllocator!
) -> CFMutableString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the string. Pass `NULL` or `kCFAllocatorDefault` to use the current default allocator.

`chars`  

The Unicode character buffer for the new `CFMutableString`. Before calling, create this buffer on the stack or heap and optionally initialize it with Unicode character data. Upon return, the created `CFString` object keeps its own copy of the pointer to this buffer. You may pass in `NULL` if there is no initial buffer being provided.

`numChars`  

The number of characters initially in the Unicode buffer pointed to by `chars`.

`capacity`  

The capacity of the external buffer (`chars`); that is, the maximum number of Unicode characters that can be stored. This value should be `0` if no initial buffer is provided.

`externalCharactersAllocator`  

The allocator to use to reallocate the external buffer when editing takes place and for deallocating the buffer when string is deallocated. If the default allocator is suitable for these purposes, pass `NULL`. To manage the buffer yourself, pass

`kCFAllocatorNull`

.

## Return Value

A new mutable string, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

This function permits you to create a `CFMutableString` object whose backing store is an external Unicode character buffer—that is, a buffer that you control (or can control) entirely. This function allows you to take advantage of the features of `CFString`, particularly the `CFMutableString` functions that add and modify character data. But at the same time you can directly add, delete, modify, and examine the characters in the buffer. You can even replace the buffer entirely. If, however, you directly modify or replace the character buffer, you should inform the `CFString` object of this change with the CFStringSetExternalCharactersNoCopy(_:_:_:_:) function.

If you mutate the character contents with the `CFString` functions, and the buffer needs to be enlarged, the `CFString` object calls the allocation callbacks specified for the allocator `externalCharactersAllocator`, or

the default allocator

if `kCFAllocatorNull` is specified.

This function should be used in special circumstances where you want to create a `CFString` wrapper around an existing, potentially large `UniChar` buffer you own. Using this function causes the `CFString` object to forgo some of its internal optimizations, so it should be avoided in general use. That is, if you want to create a `CFString` object from a small `UniChar` buffer, and you don’t need to continue owning the buffer, use one of the other creation functions (for instance CFStringCreateWithCharacters(_:_:_:)) instead.

## See Also

### CFMutableString Miscellaneous Functions

func CFStringAppend(CFMutableString!, CFString!)

Appends the characters of a string to those of a CFMutableString object.

func CFStringAppendCharacters(CFMutableString!, UnsafePointer&lt;UniChar>!, CFIndex)

Appends a buffer of Unicode characters to the character contents of a CFMutableString object.

func CFStringAppendCString(CFMutableString!, UnsafePointer&lt;CChar>!, CFStringEncoding)

Appends a C string to the character contents of a CFMutableString object.

func CFStringAppendFormatAndArguments(CFMutableString!, CFDictionary!, CFString!, CVaListPointer)

Appends a formatted string to the character contents of a CFMutableString object.

func CFStringAppendPascalString(CFMutableString!, ConstStr255Param!, CFStringEncoding)

Appends a Pascal string to the character contents of a CFMutableString object.

func CFStringCapitalize(CFMutableString!, CFLocale!)

Changes the first character in each word of a string to uppercase (if it is a lowercase alphabetical character).

func CFStringCreateMutable(CFAllocator!, CFIndex) -> CFMutableString!

Creates an empty CFMutableString object.

func CFStringCreateMutableCopy(CFAllocator!, CFIndex, CFString!) -> CFMutableString!

Creates a mutable copy of a string.

func CFStringDelete(CFMutableString!, CFRange)

Deletes a range of characters in a string.

func CFStringFindAndReplace(CFMutableString!, CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFIndex

Replaces all occurrences of a substring within a given range.

func CFStringFold(CFMutableString!, CFStringCompareFlags, CFLocale!)

Folds a given string into the form specified by optional flags.

func CFStringInsert(CFMutableString!, CFIndex, CFString!)

Inserts a string at a specified location in the character buffer of a CFMutableString object.

func CFStringLowercase(CFMutableString!, CFLocale!)

Changes all uppercase alphabetical characters in a CFMutableString to lowercase.

func CFStringNormalize(CFMutableString!, CFStringNormalizationForm)

Normalizes the string into the specified form as described in Unicode Technical Report \#15.

func CFStringPad(CFMutableString!, CFString!, CFIndex, CFIndex)

Enlarges a string, padding it with specified characters, or truncates the string.

