

- JavaScriptCore
-  JSStringRelease(\_:) 

Function

# JSStringRelease(\_:)

Releases a JavaScript string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringRelease(_ string: JSStringRef!)
```

## Parameters 

`string`  

The JSStringRef to release.

## See Also

### Creating a JavaScript String

func JSStringCreateWithCharacters(UnsafePointer&lt;JSChar>!, Int) -> JSStringRef!

Creates a JavaScript string from a buffer of Unicode characters.

typealias JSChar

A Unicode character.

func JSStringCreateWithUTF8CString(UnsafePointer&lt;CChar>!) -> JSStringRef!

Creates a JavaScript string from a null-terminated UTF-8 string.

func JSStringRetain(JSStringRef!) -> JSStringRef!

Retains a JavaScript string.

