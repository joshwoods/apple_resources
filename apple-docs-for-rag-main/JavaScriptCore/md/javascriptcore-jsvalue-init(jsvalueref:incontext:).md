

- JavaScriptCore
- JSValue
-  init(JSValueRef:inContext:) 

Initializer

# init(JSValueRef:inContext:)

Creates a JavaScript value object from the equivalent C representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
init!(
    JSValueRef value: JSValueRef!,
    inContext context: JSContext!
)
```

``` source
init!(
    jsValueRef value: JSValueRef!,
    in context: JSContext!
)
```

## Parameters 

`value`  

A C JavaScript value reference.

`context`  

The JavaScript context in which to create the value.

## Return Value

A JavaScript value object representing the same value.

## Discussion

See `JSValueRef` for the C JavaScriptCore API.

## See Also

### Working with the C JavaScriptCore API

var jsValueRef: JSValueRef!

Returns the C representation of the JavaScript value.

