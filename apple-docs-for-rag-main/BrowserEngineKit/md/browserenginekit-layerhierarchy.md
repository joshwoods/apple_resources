

- BrowserEngineKit
-  LayerHierarchy 

Class

# LayerHierarchy

An object that holds a reference to layers rendered in another process’s view.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
class LayerHierarchy
```

## Mentioned in 

Hosting browser view layers in the rendering extension

Propagating view visibility information to extension processes

## Overview

In your browser’s rendering extension, create a `LayerHierarchy` and set its layer to a CALayer that renders content to host in a view in the browser app. Get the layer hierarchy’s handle, and send it to the browser app, where you add the handle to a LayerHierarchyHostingView.

Use LayerHierarchyHostingTransactionCoordinator to synchronize updates in the view and the layer. For more information, see Hosting browser view layers in the rendering extension.

## Topics

### Creating and invalidating a layer hierarchy

init() throws

Initializes a layer hierarchy.

func invalidate()

Invalidates a layer hierarchy.

### Setting the layer

var layer: CALayer?

The layer represented by this layer hierarchy.

### Getting a handle

var handle: LayerHierarchyHandle

A reference to the layer hierarchy that you add to the hosting view.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Layer hosting

Hosting browser view layers in the rendering extension

Coordinate view-hierarchy and layer-hierarchy changes between processes.

class LayerHierarchyHostingView

A view that hosts a layer hierarchy you manage in another process.

class LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

class LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

