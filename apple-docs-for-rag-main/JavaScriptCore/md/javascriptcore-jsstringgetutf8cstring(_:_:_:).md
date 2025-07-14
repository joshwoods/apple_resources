

- JavaScriptCore
-  JSStringGetUTF8CString(\_:\_:\_:) 

Function

# JSStringGetUTF8CString(\_:\_:\_:)

Converts a JavaScript string into a null-terminated UTF-8 string, and copies the result into an external byte buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringGetUTF8CString(
    _ string: JSStringRef!,
    _ buffer: UnsafeMutablePointer!,
    _ bufferSize: Int
) -> Int
```

## Parameters 

`string`  

The source JSStringRef.

`buffer`  

The destination byte buffer to copy a null-terminated UTF-8 representation of `string` into. On return, `buffer` contains a UTF-8 string representation of `string`. If `bufferSize` is too small, `buffer` contains only partial results. If `buffer` isn’t at least `bufferSize` bytes in size, the conversion results in undefined behavior.

`bufferSize`  

The size of the external buffer in bytes.

## Return Value

The number of bytes the system writes into `buffer` (including the null-terminator byte).

## See Also

### Accessing JavaScript String Information

func JSStringGetLength(JSStringRef!) -> Int

Returns the number of Unicode characters in a JavaScript string.

func JSStringGetCharactersPtr(JSStringRef!) -> UnsafePointer&lt;JSChar>!

Returns a pointer to the Unicode character buffer that serves as the backing store for a JavaScript string.

func JSStringGetMaximumUTF8CStringSize(JSStringRef!) -> Int

Returns the maximum number of bytes a JavaScript string uses when you convert it into a null-terminated UTF-8 string.

