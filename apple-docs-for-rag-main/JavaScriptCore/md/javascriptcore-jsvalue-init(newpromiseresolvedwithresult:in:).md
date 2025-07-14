

- JavaScriptCore
- JSValue
-  init(newPromiseResolvedWithResult:in:) 

Initializer

# init(newPromiseResolvedWithResult:in:)

Creates a resolved promise object with the specified value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+

``` source
init!(
    newPromiseResolvedWithResult result: Any!,
    in context: JSContext!
)
```

## Parameters 

`result`  

The result value to pass to any reactions.

`context`  

The JSContext the resulting JSValue belongs to.

## Return Value

A JSValue that represents a new promise JavaScript object.

## Discussion

This method is equivalent to calling the following:

```
[JSValue valueWithNewPromiseFromExecutor:^(JSValue *resolve, JSValue *reject) { 
    [resolve callWithArguments:@[result]]; 
} inContext:context];
```

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

