

- JavaScriptCore
- JSContext
-  init(JSGlobalContextRef:) 

Initializer

# init(JSGlobalContextRef:)

Creates a JavaScript context object from the equivalent C representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
init!(JSGlobalContextRef jsGlobalContextRef: JSGlobalContextRef!)
```

``` source
init!(jsGlobalContextRef: JSGlobalContextRef!)
```

## Parameters 

`jsGlobalContextRef`  

A C JavaScript context reference.

## Return Value

A JavaScript context object representing the same context.

## Discussion

See `JSContextRef` for the C JavaScriptCore API.

## See Also

### Working with the C JavaScriptCore API

var jsGlobalContextRef: JSGlobalContextRef!

Returns the C representation of the JavaScript context.

