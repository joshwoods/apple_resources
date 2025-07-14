

- JavaScriptCore
-  JSValueIsDate(\_:\_:) 

Function

# JSValueIsDate(\_:\_:)

Tests whether a JavaScript value is a date.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func JSValueIsDate(
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

true if `value` is a date; otherwise, false.

## See Also

### Testing the Value’s Type

func JSValueGetType(JSContextRef!, JSValueRef!) -> JSType

Returns a JavaScript value’s type.

func JSValueIsUndefined(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value’s type is the undefined type.

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

func JSValueGetTypedArrayType(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSTypedArrayType

Returns a JavaScript value’s typed array type.

struct JSType

Constants that identify the type of a JavaScript value.

