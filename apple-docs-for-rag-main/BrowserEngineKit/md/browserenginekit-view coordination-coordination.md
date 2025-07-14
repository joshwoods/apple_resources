

- BrowserEngineKit
-  View coordination 

API Collection

# View coordination

Display content in the browser’s UI that an extension renders.

## Topics

### Layer hosting

Hosting browser view layers in the rendering extension

Coordinate view-hierarchy and layer-hierarchy changes between processes.

class LayerHierarchy

An object that holds a reference to layers rendered in another process’s view.

class LayerHierarchyHostingView

A view that hosts a layer hierarchy you manage in another process.

class LayerHierarchyHostingTransactionCoordinator

Synchronizes updates to views and layers in different processes.

class LayerHierarchyHandle

A reference to a layer hierarchy that you share between processes.

### Visibility propagation

Propagating view visibility information to extension processes

Register the extensions that contribute to preparing your browser app’s UI.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the rendering process.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the web content process.

## See Also

### Web content

Text interaction

Integrate your web browser engine asynchronously with the text system.

class BEWebAppManifest

An object that represents a web app manifest.

