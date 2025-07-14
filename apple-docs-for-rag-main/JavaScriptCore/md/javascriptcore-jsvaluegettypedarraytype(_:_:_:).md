

- JavaScriptCore
-  JSValueGetTypedArrayType(\_:\_:\_:) 

Function

# JSValueGetTypedArrayType(\_:\_:\_:)

Returns a JavaScript value’s typed array type.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
func JSValueGetTypedArrayType(
    _ ctx: JSContextRef!,
    _ value: JSValueRef!,
    _ exception: UnsafeMutablePointer!
) -> JSTypedArrayType
```

## Parameters 

`ctx`  

The execution context to use.

`value`  

The JSValueRef with the typed array type to return.

`exception`  

A pointer to a JSValueRef to store an exception in, if any. Pass `NULL` to discard any exception.

## Return Value

A value of type JSTypedArrayType that identifies the typed array type of `value`, or kJSTypedArrayTypeNone if `value` isn’t a typed array object.

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

func JSValueIsDate(JSContextRef!, JSValueRef!) -> Bool

Tests whether a JavaScript value is a date.

struct JSType

Constants that identify the type of a JavaScript value.

