

- JavaScriptCore
-  JSStringGetLength(\_:) 

Function

# JSStringGetLength(\_:)

Returns the number of Unicode characters in a JavaScript string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringGetLength(_ string: JSStringRef!) -> Int
```

## Parameters 

`string`  

The JSStringRef with the length (in Unicode characters) you want to know.

## Return Value

The number of Unicode characters in `string`.

## See Also

### Accessing JavaScript String Information

func JSStringGetCharactersPtr(JSStringRef!) -> UnsafePointer&lt;JSChar>!

Returns a pointer to the Unicode character buffer that serves as the backing store for a JavaScript string.

func JSStringGetMaximumUTF8CStringSize(JSStringRef!) -> Int

Returns the maximum number of bytes a JavaScript string uses when you convert it into a null-terminated UTF-8 string.

func JSStringGetUTF8CString(JSStringRef!, UnsafeMutablePointer&lt;CChar>!, Int) -> Int

Converts a JavaScript string into a null-terminated UTF-8 string, and copies the result into an external byte buffer.

