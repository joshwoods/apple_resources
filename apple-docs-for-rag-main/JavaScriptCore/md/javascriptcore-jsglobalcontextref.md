

- JavaScriptCore
-  JSGlobalContextRef 

Type Alias

# JSGlobalContextRef

A global JavaScript execution context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
typealias JSGlobalContextRef = OpaquePointer
```

## Discussion

A JSGlobalContextRef is a JSContextRef.

## Topics

### Creating a global context

func JSGlobalContextCreate(JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context.

func JSGlobalContextCreateInGroup(JSContextGroupRef!, JSClassRef!) -> JSGlobalContextRef!

Creates a global JavaScript execution context in the provided context group.

func JSGlobalContextRetain(JSGlobalContextRef!) -> JSGlobalContextRef!

Retains a global JavaScript execution context.

func JSGlobalContextRelease(JSGlobalContextRef!)

Releases a global JavaScript execution context.

### Managing the context’s name

func JSGlobalContextCopyName(JSGlobalContextRef!) -> JSStringRef!

Gets a copy of the name of a context.

func JSGlobalContextSetName(JSGlobalContextRef!, JSStringRef!)

Sets the remote debugging name for a context.

### Making a context inspectable

func JSGlobalContextIsInspectable(JSGlobalContextRef!) -> Bool

Returns a Boolean value that indicates whether the JavaScript context is inspectable.

func JSGlobalContextSetInspectable(JSGlobalContextRef!, Bool)

Sets a JavaScript context to be either inspectable or not inspectable.

## See Also

### JavaScriptCore Engine Interface

typealias JSContextGroupRef

A group that associates JavaScript contexts with one another.

typealias JSContextRef

A JavaScript execution context.

typealias JSStringRef

A UTF-16 character buffer.

typealias JSClassRef

A JavaScript class.

