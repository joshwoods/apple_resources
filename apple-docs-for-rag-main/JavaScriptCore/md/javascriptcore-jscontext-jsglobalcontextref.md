

- JavaScriptCore
- JSContext
-  jsGlobalContextRef 

Instance Property

# jsGlobalContextRef

Returns the C representation of the JavaScript context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var jsGlobalContextRef: JSGlobalContextRef! { get }
```

## Discussion

See `JSContextRef` for the C JavaScriptCore API.

## See Also

### Working with the C JavaScriptCore API

init!(JSGlobalContextRef: JSGlobalContextRef!)

Creates a JavaScript context object from the equivalent C representation.

