

- BrowserEngineKit
- LayerHierarchy
-  invalidate() 

Instance Method

# invalidate()

Invalidates a layer hierarchy.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
func invalidate()
```

## Mentioned in 

Hosting browser view layers in the rendering extension

## Overview

When you call this method, the layer hierarchy can’t be hosted in a LayerHierarchyHostingView. Communicate with the browser app to remove the hosting view from its superview.

## See Also

### Creating and invalidating a layer hierarchy

init() throws

Initializes a layer hierarchy.

