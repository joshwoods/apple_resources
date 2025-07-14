

- JavaScriptCore
-  JSClassRef 

Type Alias

# JSClassRef

A JavaScript class.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSClassRef = OpaquePointer
```

## Discussion

Use this type with JSObjectMake(_:_:_:) to construct objects with custom behavior.

## See Also

### JavaScriptCore Engine Interface

typealias JSContextGroupRef

A group that associates JavaScript contexts with one another.

typealias JSContextRef

A JavaScript execution context.

typealias JSGlobalContextRef

A global JavaScript execution context.

typealias JSStringRef

A UTF-16 character buffer.

