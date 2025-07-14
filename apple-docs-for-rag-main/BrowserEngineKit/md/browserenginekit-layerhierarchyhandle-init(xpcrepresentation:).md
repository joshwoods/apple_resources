

- BrowserEngineKit
- LayerHierarchyHandle
-  init(xpcRepresentation:) 

Initializer

# init(xpcRepresentation:)

Creates a handle from a representation received in an XPC message.

iOS 17.4+iPadOS 17.4+

``` source
init(xpcRepresentation: xpc_object_t?) throws
```

## Parameters 

`xpcRepresentation`  

A representation of the handle, encoded as an XPC object.

## See Also

### Interprocess communication

init?(coder: NSCoder)

Creates a handle from an encoded representation.

func createXPCRepresentation() -> xpc_object_t

Creates an object representing this handle that you send to another process in an XPC message.

