

- JavaScriptCore
-  JSStringRetain(\_:) 

Function

# JSStringRetain(\_:)

Retains a JavaScript string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringRetain(_ string: JSStringRef!) -> JSStringRef!
```

## Parameters 

`string`  

The JSStringRef to retain.

## Return Value

A JSStringRef that is the same as `string`.

## See Also

### Creating a JavaScript String

func JSStringCreateWithCharacters(UnsafePointer&lt;JSChar>!, Int) -> JSStringRef!

Creates a JavaScript string from a buffer of Unicode characters.

typealias JSChar

A Unicode character.

func JSStringCreateWithUTF8CString(UnsafePointer&lt;CChar>!) -> JSStringRef!

Creates a JavaScript string from a null-terminated UTF-8 string.

func JSStringRelease(JSStringRef!)

Releases a JavaScript string.

