

- JavaScriptCore
- JSValue
-  init(newPromiseIn:fromExecutor:) 

Initializer

# init(newPromiseIn:fromExecutor:)

Creates a promise object using the specified executor callback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+

``` source
init!(
    newPromiseIn context: JSContext!,
    fromExecutor callback: ((JSValue?, JSValue?) -> Void)!
)
```

## Parameters 

`context`  

The JSContext the resulting JSValue belongs to.

`callback`  

A callback block to invoke during initialization of the promise object. The `resolve` and `reject` parameters are functions that you can call to notify any pending reactions about the state of the new promise object.

## Return Value

A JSValue that represents a new promise JavaScript object.

## Discussion

This method is equivalent to calling the `Promise()` constructor in JavaScript.

The `resolve` and `reject` callbacks each typically take a single value, which they forward to all relevant pending reactions. While inside the executor callback, `context` acts as if it is in any other callback, except `calleeFunction` is `nil`. This also means you can access the new promise object using `[context thisValue]`.

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

init!(newErrorFromMessage: String!, in: JSContext!)

Creates a JavaScript error value with the specified error message.

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

