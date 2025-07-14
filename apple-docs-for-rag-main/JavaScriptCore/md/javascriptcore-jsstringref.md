

- JavaScriptCore
-  JSStringRef 

Type Alias

# JSStringRef

A UTF-16 character buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSStringRef = OpaquePointer
```

## Discussion

This is the fundamental string representation in JavaScript.

## Topics

### Creating a JavaScript String

func JSStringCreateWithCharacters(UnsafePointer&lt;JSChar>!, Int) -> JSStringRef!

Creates a JavaScript string from a buffer of Unicode characters.

typealias JSChar

A Unicode character.

func JSStringCreateWithUTF8CString(UnsafePointer&lt;CChar>!) -> JSStringRef!

Creates a JavaScript string from a null-terminated UTF-8 string.

func JSStringRetain(JSStringRef!) -> JSStringRef!

Retains a JavaScript string.

func JSStringRelease(JSStringRef!)

Releases a JavaScript string.

### Accessing JavaScript String Information

func JSStringGetLength(JSStringRef!) -> Int

Returns the number of Unicode characters in a JavaScript string.

func JSStringGetCharactersPtr(JSStringRef!) -> UnsafePointer&lt;JSChar>!

Returns a pointer to the Unicode character buffer that serves as the backing store for a JavaScript string.

func JSStringGetMaximumUTF8CStringSize(JSStringRef!) -> Int

Returns the maximum number of bytes a JavaScript string uses when you convert it into a null-terminated UTF-8 string.

func JSStringGetUTF8CString(JSStringRef!, UnsafeMutablePointer&lt;CChar>!, Int) -> Int

Converts a JavaScript string into a null-terminated UTF-8 string, and copies the result into an external byte buffer.

### Comparing JavaScript Strings

func JSStringIsEqual(JSStringRef!, JSStringRef!) -> Bool

Tests whether two JavaScript strings match.

func JSStringIsEqualToUTF8CString(JSStringRef!, UnsafePointer&lt;CChar>!) -> Bool

Tests whether a JavaScript string matches a null-terminated UTF-8 string.

### Converting to and from Core Foundation Strings

func JSStringCreateWithCFString(CFString!) -> JSStringRef!

Creates a JavaScript string from a Core Foundation string.

func JSStringCopyCFString(CFAllocator!, JSStringRef!) -> CFString!

Creates a Core Foundation string from a JavaScript string.

## See Also

### JavaScriptCore Engine Interface

typealias JSContextGroupRef

A group that associates JavaScript contexts with one another.

typealias JSContextRef

A JavaScript execution context.

typealias JSGlobalContextRef

A global JavaScript execution context.

typealias JSClassRef

A JavaScript class.

