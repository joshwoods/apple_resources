

- JavaScriptCore
-  JSStringCreateWithUTF8CString(\_:) 

Function

# JSStringCreateWithUTF8CString(\_:)

Creates a JavaScript string from a null-terminated UTF-8 string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringCreateWithUTF8CString(_ string: UnsafePointer!) -> JSStringRef!
```

## Parameters 

`string`  

The null-terminated UTF-8 string to copy into the new JSStringRef.

## Return Value

A JSStringRef that contains `string`. Ownership follows The Create Rule.

## See Also

### Creating a JavaScript String

func JSStringCreateWithCharacters(UnsafePointer&lt;JSChar>!, Int) -> JSStringRef!

Creates a JavaScript string from a buffer of Unicode characters.

typealias JSChar

A Unicode character.

func JSStringRetain(JSStringRef!) -> JSStringRef!

Retains a JavaScript string.

func JSStringRelease(JSStringRef!)

Releases a JavaScript string.

