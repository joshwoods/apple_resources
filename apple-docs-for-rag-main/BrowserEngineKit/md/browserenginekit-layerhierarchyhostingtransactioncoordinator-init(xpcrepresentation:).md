

- BrowserEngineKit
- LayerHierarchyHostingTransactionCoordinator
-  init(xpcRepresentation:) 

Initializer

# init(xpcRepresentation:)

Creates a transaction coordinator from an XPC object.

iOS 17.4+iPadOS 17.4+

``` source
init(xpcRepresentation: xpc_object_t?) throws
```

## Parameters 

`xpcRepresentation`  

An XPC object describing the transaction coordinator to initialize.

## Overview

This initializer can fail and throw an error if the `xpcRepresentation` doesn’t represent a transaction coordinator.

## See Also

### Interprocess communication

init?(coder: NSCoder)

Creates a transaction coordinator from an encoded representation.

func createXPCRepresentation() -> xpc_object_t

Creates a representation of the transaction coordinator you send to another process.

