

- JavaScriptCore
-  JSValueMakeFromJSONString(\_:\_:) 

Function

# JSValueMakeFromJSONString(\_:\_:)

Creates a JavaScript value from a JSON-formatted string.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func JSValueMakeFromJSONString(
    _ ctx: JSContextRef!,
    _ string: JSStringRef!
) -> JSValueRef!
```

## Parameters 

`ctx`  

The execution context to use.

`string`  

The JSStringRef that contains the JSON string to parse.

## Return Value

A JSValueRef that contains the parsed value, or `NULL` if the input is invalid.

## See Also

### Converting to and from JSON-Formatted Strings

func JSValueCreateJSONString(JSContextRef!, JSValueRef!, UInt32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Creates a JavaScript string that contains the JSON-serialized representation of a JavaScript value.

