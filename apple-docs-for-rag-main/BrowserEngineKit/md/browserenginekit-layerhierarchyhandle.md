

- BrowserEngineKit
-  LayerHierarchyHandle 

Class

# LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

iOS 17.4+iPadOS 17.4+

``` source
class LayerHierarchyHandle
```

## Mentioned in 

Hosting browser view layers in the rendering extension

## Topics

### Interprocess communication

init?(coder: NSCoder)

Creates a handle from an encoded representation.

init(xpcRepresentation: xpc_object_t?) throws

Creates a handle from a representation received in an XPC message.

func createXPCRepresentation() -> xpc_object_t

Creates an object representing this handle that you send to another process in an XPC message.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Layer hosting

Hosting browser view layers in the rendering extension

Coordinate view-hierarchy and layer-hierarchy changes between processes.

class LayerHierarchy

An object that holds a reference to layers rendered in another process’s view.

class LayerHierarchyHostingView

A view that hosts a layer hierarchy you manage in another process.

class LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

