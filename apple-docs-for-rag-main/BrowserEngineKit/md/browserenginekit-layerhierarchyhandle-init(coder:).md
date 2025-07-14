

- BrowserEngineKit
- LayerHierarchyHandle
-  init(coder:) 

Initializer

# init(coder:)

Creates a handle from an encoded representation.

iOS 17.4+iPadOS 17.4+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An object that contains data that describes the handle to create.

## See Also

### Interprocess communication

init(xpcRepresentation: xpc_object_t?) throws

Creates a handle from a representation received in an XPC message.

func createXPCRepresentation() -> xpc_object_t

Creates an object representing this handle that you send to another process in an XPC message.

