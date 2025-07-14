

- BrowserEngineKit
- LayerHierarchyHostingTransactionCoordinator
-  init(coder:) 

Initializer

# init(coder:)

Creates a transaction coordinator from an encoded representation.

iOS 17.4+iPadOS 17.4+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An object that contains the encoded representation of the transaction coordinator.

## Overview

This initializer can fail and return `nil` if it can’t decode the data it needs from the `coder`.

## See Also

### Interprocess communication

init(xpcRepresentation: xpc_object_t?) throws

Creates a transaction coordinator from an XPC object.

func createXPCRepresentation() -> xpc_object_t

Creates a representation of the transaction coordinator you send to another process.

