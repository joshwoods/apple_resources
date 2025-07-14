

- JavaScriptCore
- JSValue
-  init(newErrorFromMessage:in:) 

Initializer

# init(newErrorFromMessage:in:)

Creates a JavaScript error value with the specified error message.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init!(
    newErrorFromMessage message: String!,
    in context: JSContext!
)
```

## Parameters 

`message`  

The error message for the error object.

`context`  

The JavaScript context in which to create the value.

## Return Value

A new JavaScript error value.

## Discussion

Calling this method creates a JavaScript `Error` object, and is equivalent to calling the `Error` constructor (for example, `new Error("message")`) in JavaScript.

## See Also

### Creating JavaScript Values

init!(object: Any!, in: JSContext!)

Creates a JavaScript value by converting the specified native object.

init!(bool: Bool, in: JSContext!)

Creates a JavaScript representation of the specified Boolean value.

init!(double: Double, in: JSContext!)

Creates a JavaScript representation of the specified floating-point value.

init!(int32: Int32, in: JSContext!)

Creates a JavaScript representation of the specified signed integer value.

init!(uInt32: UInt32, in: JSContext!)

Creates a JavaScript representation of the specified unsigned integer value.

init!(newObjectIn: JSContext!)

Creates a new, empty JavaScript object value.

init!(newArrayIn: JSContext!)

Creates a new, empty JavaScript array value.

init!(newRegularExpressionFromPattern: String!, flags: String!, in: JSContext!)

Creates a JavaScript regular expression value from the specified pattern.

init!(undefinedIn: JSContext!)

Creates a JavaScript `undefined` value.

init!(nullIn: JSContext!)

Creates a JavaScript `null` value.

init!(point: CGPoint, inContext: JSContext!)

Creates a JavaScript representation of the specified point.

init!(range: NSRange, inContext: JSContext!)

Creates a JavaScript representation of the specified range.

init!(rect: CGRect, inContext: JSContext!)

Creates a JavaScript representation of the specified rectangle.

init!(size: CGSize, inContext: JSContext!)

Creates a JavaScript representation of the specified width and height.

init!(newSymbolFromDescription: String!, in: JSContext!)

Creates a unique symbol object.

