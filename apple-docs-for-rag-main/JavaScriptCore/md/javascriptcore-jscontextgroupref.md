

- JavaScriptCore
-  JSContextGroupRef 

Type Alias

# JSContextGroupRef

A group that associates JavaScript contexts with one another.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSContextGroupRef = OpaquePointer
```

## Discussion

Contexts in the same group may share and exchange JavaScript objects.

## Topics

### Accessing the Content Group

func JSContextGetGroup(JSContextRef!) -> JSContextGroupRef!

Gets the context group that a JavaScript execution context belongs to.

## See Also

### JavaScriptCore Engine Interface

typealias JSContextRef

A JavaScript execution context.

typealias JSGlobalContextRef

A global JavaScript execution context.

typealias JSStringRef

A UTF-16 character buffer.

typealias JSClassRef

A JavaScript class.

