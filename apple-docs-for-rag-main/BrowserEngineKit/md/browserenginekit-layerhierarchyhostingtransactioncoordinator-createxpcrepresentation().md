

- BrowserEngineKit
- LayerHierarchyHostingTransactionCoordinator
-  createXPCRepresentation() 

Instance Method

# createXPCRepresentation()

Creates a representation of the transaction coordinator you send to another process.

iOS 17.4+iPadOS 17.4+

``` source
func createXPCRepresentation() -> xpc_object_t
```

## See Also

### Interprocess communication

init?(coder: NSCoder)

Creates a transaction coordinator from an encoded representation.

init(xpcRepresentation: xpc_object_t?) throws

Creates a transaction coordinator from an XPC object.

