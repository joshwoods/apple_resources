

- BrowserEngineKit
- LayerHierarchyHandle
-  createXPCRepresentation() 

Instance Method

# createXPCRepresentation()

Creates an object representing this handle that you send to another process in an XPC message.

iOS 17.4+iPadOS 17.4+

``` source
func createXPCRepresentation() -> xpc_object_t
```

## See Also

### Interprocess communication

init?(coder: NSCoder)

Creates a handle from an encoded representation.

init(xpcRepresentation: xpc_object_t?) throws

Creates a handle from a representation received in an XPC message.

