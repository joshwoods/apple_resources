

- JavaScriptCore
-  JSStringCreateWithCharacters(\_:\_:) 

Function

# JSStringCreateWithCharacters(\_:\_:)

Creates a JavaScript string from a buffer of Unicode characters.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSStringCreateWithCharacters(
    _ chars: UnsafePointer!,
    _ numChars: Int
) -> JSStringRef!
```

## Parameters 

`chars`  

The buffer of Unicode characters to copy into the new JSStringRef.

`numChars`  

The number of characters to copy from the buffer that `chars` points to.

## Return Value

A JSStringRef that contains `chars`. Ownership follows The Create Rule.

## See Also

### Creating a JavaScript String

typealias JSChar

A Unicode character.

func JSStringCreateWithUTF8CString(UnsafePointer&lt;CChar>!) -> JSStringRef!

Creates a JavaScript string from a null-terminated UTF-8 string.

func JSStringRetain(JSStringRef!) -> JSStringRef!

Retains a JavaScript string.

func JSStringRelease(JSStringRef!)

Releases a JavaScript string.

