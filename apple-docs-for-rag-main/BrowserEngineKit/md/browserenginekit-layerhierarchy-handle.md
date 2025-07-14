

- BrowserEngineKit
- LayerHierarchy
-  handle 

Instance Property

# handle

A reference to the layer hierarchy that you add to the hosting view.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
var handle: LayerHierarchyHandle { get }
```

## Overview

Get the handle in your extension process, then use XPC to send it to the browser app. In the browser app, add the handle to a LayerHierarchyHostingView.

