

- BrowserEngineKit
- View coordination
-  Hosting browser view layers in the rendering extension 

Article

# Hosting browser view layers in the rendering extension

Coordinate view-hierarchy and layer-hierarchy changes between processes.

## Overview

When your browser app’s alternative browser engine is split between different extensions, you coordinate those extensions to prepare the browser’s UI. For example, your browser controls are rendered by the host app, and media is streamed in the rendering extension.

Create layer hierarchies to manage CALayer objects in the rendering extension. Host those layers in a hosting view that you add to your view hierarchy. Indicate to the operating system that the view contains hosted layers, and coordinate changes to the layer hierarchy between your host app and rendering extension.

Note

If you create images or render content to an IOSurfaceRef in your rendering extension, you can send that object to the host object over XPC and don’t need to render a hosted layer. If you render UI in a web content extension, use `IOSurfaceRef` in the rendering extension, or generate any UI in the rendering extension other than a `CALayer`, you need to create a visibility propagation interaction for the view in the host app. For more information, see Propagating view visibility information to extension processes.

### Create a hosted layer hierarchy and a hosting view

In the extension process that prepares the rendered content, create a LayerHierarchy and set its layer to the root layer in the content’s layer hierarchy. Get the layer hierarchy’s LayerHierarchyHandle, and send it over XPC to your browser app:

```
let layer: CALayer = // Create your content layer.
if let hierarchy = try? LayerHierarchy() {
  hierarchy.layer = layer
  let xpcHandle = hierarchy.handle.createXPCRepresentation()
  // Send the handle to your browser app, using XPC.
  // Retain the hierarchy while your app's using it.
  self.storedHierarchy = hierarchy 
}
```

For more information on using XPC in browser apps and extensions, see Using XPC to communicate with browser extensions.

In the host app, add the handle to a LayerHierarchyHostingView:

```
let xpcHandle: xpc_object_t = // Get the handle from an XPC message.
if let handle = try? LayerHierarchyHandle(xpcRepresentation: xpcHandle) {
  let hostingView = LayerHierarchyHostingView()
  hostingView.handle = handle
  // Prepare the view for display.
  self.view.addSubview(hostingView)
}
```

### Coordinate updates to the view and layer hierarchy

When you need to make changes to the view hierarchy that involve the `LayerHierarchyHostingView`, coordinate the changes between the host app and the extension that controls the hosted layers.

You can initiate the update in either the host app or the extension. To initiate the update in the host app, create a LayerHierarchyHostingTransactionCoordinator, add the `LayerHierarchyHostingView`, and make changes to the view or its superviews. Use XPC to send a representation of the `LayerHierarchyHostingTransactionCoordinator` to the extension, then commit() the transaction coordinator.

```
if let coordinator = try? LayerHierarchyHostingTransactionCoordinator() {
  coordinator.add(hostingView)
  // Make changes to the hosting view or its view hierarchy.
  let xpcCoordinator = coordinator.createXPCRepresentation()
  // Send the xpcCoordinator to the extension that's managing the view's layer.
  coordinator.commit()
}
```

In the extension, use the XPC representation of the coordinator to create a `LayerHierarchyHostingTransactionCoordinator`, and add the layer hierarchy to the transaction coordinator. Make changes to the layer or its sublayers, then commit the transaction coordinator.

```
let xpcCoordinator: xpc_object_t = // Get the object from an XPC message.
if let coordinator = try? LayerHostingHierarchyTransactionCoordinator(xpcRepresentation: xpcCoordinator) {
  coordinator.add(self.storedHierarchy)
  // Make change to the layer or its sublayers.
  coordinator.commit()
}
```

Note

You need to add layers or views to the transaction coordinator before you manipulate those layers or views. Commit the transaction coordinator as the last action in the process of updating the views or layers, after you send the XPC representation of the transaction coordinator to the other process.

To initiate the update in the extension, create a `LayerHostingHierarchyTransactionCoordinator` to track changes to the layer hierarchy, then send it to the host app to create the transaction coordinator you use to track changes to the view hierarchy.

`LayerHierarchyHostingTransactionCoordinator` doesn’t communicate any information about the updates you make to the views and layers you add to them. Use your XPC communication channel to send the context of any changes to views and layers between your browser app and extension processes, along with the transaction coordinator.

Keep the lifetime of transaction coordinators — from initialization until you call commit() — as short as possible to avoid making your UI unresponsive. The operating system expects you to call `commit()` within a short interval, and stops coordinating transactions if you exceed this duration. A person using your browser app experiences this as glitches in your app’s user interface and inconsistent animations.

### Dispose of views with hosted layers

When the layer that’s rendered in a `LayerHierarchyHostingView` is no longer needed, call invalidate() on the layer hierarchy in the extension. Send an XPC message to notify the browser to remove the view from its superview. When you invalidate a `LayerHierarchy`, you can no longer use that hierarchy or its hosting view.

## See Also

### Layer hosting

class LayerHierarchy

An object that holds a reference to layers rendered in another process’s view.

class LayerHierarchyHostingView

A view that hosts a layer hierarchy you manage in another process.

class LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

class LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

