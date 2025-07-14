

- JavaScriptCore
-  JSValueToStringCopy(\_:\_:\_:) 

Function

# JSValueToStringCopy(\_:\_:\_:)

Converts a JavaScript value to a string and copies the result into a JavaScript string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueToStringCopy(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ exception: UnsafeMutablePointer!
) -> JSStringRef!
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to convert.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A JSStringRef with the result of conversion, or `NULL` if the system throws an exception. Ownership follows The Create Rule.

## See Also

### Converting to Primitive Values

func JSValueToBoolean(JSContextRef!, JSValueRef!) -> Bool

Converts a JavaScript value to a Boolean and returns the resulting Boolean.

func JSValueToNumber(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Double

Converts a JavaScript value to a number and returns the resulting number.

func JSValueToObject(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Converts a JavaScript value to an object and returns the resulting object.

