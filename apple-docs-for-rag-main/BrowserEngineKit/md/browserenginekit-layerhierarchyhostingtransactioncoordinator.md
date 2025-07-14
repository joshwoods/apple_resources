

- BrowserEngineKit
-  LayerHierarchyHostingTransactionCoordinator 

Class

# LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

iOS 17.4+iPadOS 17.4+

``` source
class LayerHierarchyHostingTransactionCoordinator
```

## Mentioned in 

Hosting browser view layers in the rendering extension

## Topics

### Creating a transaction coordinator

init() throws

may fail if a connection to the render server cannot be established

### Interprocess communication

init?(coder: NSCoder)

Creates a transaction coordinator from an encoded representation.

init(xpcRepresentation: xpc_object_t?) throws

Creates a transaction coordinator from an XPC object.

func createXPCRepresentation() -> xpc_object_t

Creates a representation of the transaction coordinator you send to another process.

### Synchronize transactions

func add(LayerHierarchyHostingView)

Notifies the transaction coordinator to start coordinating transactions for the given view.

func add(LayerHierarchy)

a signal to coordinate transactions involving `layerHierarchy` from now until `commit` is called

func commit()

`commit` must be called on *every* instance and it must be the last call to each instance. note that it does not commit `CATransaction`s but rather commits the coordination of transactions in the render server. note that coordinators should have as constrained a lifespan as possible and will timeout if held open too long.

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

class LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

