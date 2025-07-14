

- JavaScriptCore
-  JSValueRef 

Type Alias

# JSValueRef

A JavaScript value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSValueRef = OpaquePointer
```

## Discussion

This is the base type for all JavaScript values, and polymorphic functions on them.

## Topics

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

func JSValueGetTypedArrayType(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSTypedArrayType

Returns a JavaScript value’s typed array type.

struct JSType

Constants that identify the type of a JavaScript value.

### Creating Values

func JSValueMakeUndefined(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the undefined type.

func JSValueMakeNull(JSContextRef!) -> JSValueRef!

Creates a JavaScript value of the null type.

func JSValueMakeBoolean(JSContextRef!, Bool) -> JSValueRef!

Creates a JavaScript Boolean value.

func JSValueMakeNumber(JSContextRef!, Double) -> JSValueRef!

Creates a JavaScript value of the number type.

func JSValueMakeString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the string type.

func JSValueMakeSymbol(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value of the symbol type.

### Converting to Primitive Values

func JSValueToBoolean(JSContextRef!, JSValueRef!) -> Bool

Converts a JavaScript value to a Boolean and returns the resulting Boolean.

func JSValueToNumber(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Double

Converts a JavaScript value to a number and returns the resulting number.

func JSValueToStringCopy(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Converts a JavaScript value to a string and copies the result into a JavaScript string.

func JSValueToObject(JSContextRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSObjectRef!

Converts a JavaScript value to an object and returns the resulting object.

### Converting to and from JSON-Formatted Strings

func JSValueMakeFromJSONString(JSContextRef!, JSStringRef!) -> JSValueRef!

Creates a JavaScript value from a JSON-formatted string.

func JSValueCreateJSONString(JSContextRef!, JSValueRef!, UInt32, UnsafeMutablePointer&lt;JSValueRef?>!) -> JSStringRef!

Creates a JavaScript string that contains the JSON-serialized representation of a JavaScript value.

### Comparing Values

func JSValueIsEqual(JSContextRef!, JSValueRef!, JSValueRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether two JavaScript values are equal.

func JSValueIsStrictEqual(JSContextRef!, JSValueRef!, JSValueRef!) -> Bool

Tests whether two JavaScript values are strict equal.

func JSValueIsInstanceOfConstructor(JSContextRef!, JSValueRef!, JSObjectRef!, UnsafeMutablePointer&lt;JSValueRef?>!) -> Bool

Tests whether a JavaScript value is an object that the specified constructor creates.

### Supporting Garbage Collection

func JSValueProtect(JSContextRef!, JSValueRef!)

Protects a JavaScript value from garbage collection.

func JSValueUnprotect(JSContextRef!, JSValueRef!)

Unprotects a JavaScript value from garbage collection.

## See Also

### JavaScript Data Types

typealias JSObjectRef

A JavaScript object.

