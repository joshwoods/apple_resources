

- JavaScriptCore
-  JSValueToNumber(\_:\_:\_:) 

Function

# JSValueToNumber(\_:\_:\_:)

Converts a JavaScript value to a number and returns the resulting number.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueToNumber(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ exception: UnsafeMutablePointer!
) -> Double
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to convert.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

The numeric result of conversion, or `NaN` if the system throws an exception.

## See Also

### Converting to Primitive Values

func JSValueToBoolean(JSContextRef!, JSValueRef!) -> Bool

Converts a JavaScript value to a Boolean and returns the resulting Boolean.

func JSValueToStringCopy(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Converts a JavaScript value to a string and copies the result into a JavaScript string.

func JSValueToObject(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Converts a JavaScript value to an object and returns the resulting object.

