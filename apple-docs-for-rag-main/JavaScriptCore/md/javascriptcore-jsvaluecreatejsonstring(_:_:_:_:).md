

- JavaScriptCore
-  JSValueCreateJSONString(\_:\_:\_:\_:) 

Function

# JSValueCreateJSONString(\_:\_:\_:\_:)

Creates a JavaScript string that contains the JSON-serialized representation of a JavaScript value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func JSValueCreateJSONString(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ indent: UInt32,
    _ exception: UnsafeMutablePointer!
) -> JSStringRef!
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The value to serialize.

`indent`  

The number of spaces to indent when nesting. If `0`, the resulting JSON string doesn’t contain new lines. The size of the indent clamps to 10 spaces.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A JSStringRef with the result of serialization, or `NULL` if the system throws an exception.

## See Also

### Converting to and from JSON-Formatted Strings

func JSValueMakeFromJSONString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value from a JSON-formatted string.

