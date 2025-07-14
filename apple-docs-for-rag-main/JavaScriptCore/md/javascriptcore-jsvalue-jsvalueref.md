

- JavaScriptCore
- JSValue
-  jsValueRef 

Instance Property

# jsValueRef

Returns the C representation of the JavaScript value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var jsValueRef: JSValueRef! { get }
```

## Discussion

See `JSValueRef` for the C JavaScriptCore API.

## See Also

### Working with the C JavaScriptCore API

init!(JSValueRef: JSValueRef!, inContext: JSContext!)

Creates a JavaScript value object from the equivalent C representation.

