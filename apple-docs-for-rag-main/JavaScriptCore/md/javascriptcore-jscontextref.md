

- JavaScriptCore
-  JSContextRef 

Type Alias

# JSContextRef

A JavaScript execution context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSContextRef = OpaquePointer
```

## Discussion

This holds the global object and other execution state.

## Topics

### Creating a Context Group

func JSContextGroupCreate() -> JSContextGroupRef!

Creates a JavaScript context group.

func JSContextGroupRetain(JSContextGroupRef!) -> JSContextGroupRef!

Retains a JavaScript context group.

func JSContextGroupRelease(JSContextGroupRef!)

Releases a JavaScript context group.

### Accessing the Global Context

func JSContextGetGlobalContext(JSContextRef!) -> JSGlobalContextRef!

Gets the global context of a JavaScript execution context.

## See Also

### JavaScriptCore Engine Interface

typealias JSContextGroupRef

A group that associates JavaScript contexts with one another.

typealias JSGlobalContextRef

A global JavaScript execution context.

typealias JSStringRef

A UTF-16 character buffer.

typealias JSClassRef

A JavaScript class.

