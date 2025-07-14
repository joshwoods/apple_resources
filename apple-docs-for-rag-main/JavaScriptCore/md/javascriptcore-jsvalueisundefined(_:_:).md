

- JavaScriptCore
-  JSValueIsUndefined(\_:\_:) 

Function

# JSValueIsUndefined(\_:\_:)

Tests whether a JavaScript value’s type is the undefined type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func JSValueIsUndefined(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!
) -> Bool
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef to test.

## Return Value

true if the type of `value` is the undefined type; otherwise, false.

## See Also

### Testing the Value’s Type

func JSValueGetType(JSContextRef!, JSValueRef!) -> JSType

Returns a JavaScript value’s type.

func JSValueIsNull(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the null type.

func JSValueIsBoolean(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value is Boolean.

func JSValueIsNumber(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the number type.

func JSValueIsString(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the string type.

func JSValueIsSymbol(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the symbol type.

func JSValueIsObject(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the object type.

func JSValueIsObjectOfClass(JSContextRef!, JSValueRef!, JSClassRef!) -> Bool

Tests whether a JavaScript value is an object with a specified class in its class chain.

func JSValueIsArray(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value is an array.

func JSValueIsDate(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value is a date.

func JSValueGetTypedArrayType(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSTypedArrayType

Returns a JavaScript value’s typed array type.

struct JSType

Constants that identify the type of a JavaScript value.

