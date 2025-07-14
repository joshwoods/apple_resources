

- BrowserEngineKit
- LayerHierarchyHostingTransactionCoordinator
-  init() 

Initializer

# init()

may fail if a connection to the render server cannot be established

iOS 17.4+iPadOS 17.4+

``` source
init() throws
```

## Discussion

Creates a transaction coordinator.

## Overview

This initializer can fail and throw an error if the process can’t get a connection to the operating system’s Core Animation rendering server.

