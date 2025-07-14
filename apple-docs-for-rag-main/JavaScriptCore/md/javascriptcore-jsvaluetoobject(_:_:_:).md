

- JavaScriptCore
-  JSValueToObject(\_:\_:\_:) 

Function

# JSValueToObject(\_:\_:\_:)

Converts a JavaScript value to an object and returns the resulting object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueToObject(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ exception: UnsafeMutablePointer!
) -> JSObjectRef!
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to convert.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

The JSObjectRef result of conversion, or `NULL` if the system throws an exception.

## See Also

### Converting to Primitive Values

func JSValueToBoolean(JSContextRef!, JSValueRef!) -> Bool

Converts a JavaScript value to a Boolean and returns the resulting Boolean.

func JSValueToNumber(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Double

Converts a JavaScript value to a number and returns the resulting number.

func JSValueToStringCopy(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Converts a JavaScript value to a string and copies the result into a JavaScript string.

