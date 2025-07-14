

- JavaScriptCore
-  JSValueToBoolean(\_:\_:) 

Function

# JSValueToBoolean(\_:\_:)

Converts a JavaScript value to a Boolean and returns the resulting Boolean.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueToBoolean(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to convert.

## Return Value

The Boolean result of conversion.

## See Also

### Converting to Primitive Values

func JSValueToNumber(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Double

Converts a JavaScript value to a number and returns the resulting number.

func JSValueToStringCopy(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Converts a JavaScript value to a string and copies the result into a JavaScript string.

func JSValueToObject(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Converts a JavaScript value to an object and returns the resulting object.

