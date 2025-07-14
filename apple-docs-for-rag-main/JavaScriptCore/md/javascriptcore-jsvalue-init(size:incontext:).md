

- JavaScriptCore
- JSValue
-  init(size:inContext:) 

Initializer

# init(size:inContext:)

Creates a JavaScript representation of the specified width and height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
init!(
    size: CGSize,
    inContext context: JSContext!
)
```

``` source
init!(
    size: CGSize,
    in context: JSContext!
)
```

## Parameters 

`size`  

A CoreGraphics size structure.

`context`  

The JavaScript context in which to create the value.

## Return Value

A JavaScript object representing the specified size.

## Discussion

Converting a rectangle creates a JavaScript object value with fields named `width` and `height`.

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

init!(newSymbolFromDescription: String!, in: JSContext!)

Creates a unique symbol object.

