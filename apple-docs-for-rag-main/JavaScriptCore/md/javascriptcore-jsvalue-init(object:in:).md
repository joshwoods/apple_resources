

- JavaScriptCore
- JSValue
-  init(object:in:) 

Initializer

# init(object:in:)

Creates a JavaScript value by converting the specified native object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init!(
    object value: Any!,
    in context: JSContext!
)
```

## Parameters 

`value`  

The Objective-C or Swift object to be made available to JavaScript.

`context`  

The JavaScript context in which to create the value.

## Return Value

A new JavaScript value representing the object.

## Discussion

Converting a native object creates a JavaScript object, including a constructor and prototype chain that reflects the object’s inheritance in the Objective-C or Swift type hierarchy. By default, properties and methods on the converted object are not exposed to JavaScript: to choose which properties and methods should be visible to JavaScript, see JSExport.

Creating a JSValue instance that wraps a native object retains the underlying Objective-C or Swift object.

## See Also

### Creating JavaScript Values

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

init!(newSymbolFromDescription: String!, in: JSContext!)

Creates a unique symbol object.

