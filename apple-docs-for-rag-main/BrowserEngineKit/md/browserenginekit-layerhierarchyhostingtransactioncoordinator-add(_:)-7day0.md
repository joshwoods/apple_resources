

- BrowserEngineKit
- LayerHierarchyHostingTransactionCoordinator
-  add(\_:) 

Instance Method

# add(\_:)

Notifies the transaction coordinator to start coordinating transactions for the given view.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
func add(_ hostingView: LayerHierarchyHostingView)
```

## Parameters 

`hostingView`  

The view to coordinate transactions for.

## Overview

The transaction coordinator coordinates any transactions involving `hostingView` until you call commit().

## See Also

### Synchronize transactions

func add(LayerHierarchy)

a signal to coordinate transactions involving `layerHierarchy` from now until `commit` is called

func commit()

`commit` must be called on *every* instance and it must be the last call to each instance. note that it does not commit `CATransaction`s but rather commits the coordination of transactions in the render server. note that coordinators should have as constrained a lifespan as possible and will timeout if held open too long.

