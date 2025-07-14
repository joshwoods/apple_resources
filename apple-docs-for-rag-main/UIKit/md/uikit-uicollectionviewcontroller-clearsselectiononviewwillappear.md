

- UIKit
- UICollectionViewController
-  clearsSelectionOnViewWillAppear 

Instance Property

# clearsSelectionOnViewWillAppear

A Boolean value indicating if the controller clears the selection when the collection view appears.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var clearsSelectionOnViewWillAppear: Bool { get set }
```

## Discussion

The default value of this property is true. When true, the collection view controller clears the collection view’s current selection when it receives a viewWillAppear(_:) message. Setting this property to false preserves the selection.

## See Also

### Configuring the collection view behavior

var installsStandardGestureForInteractiveMovement: Bool

A Boolean value indicating whether the collection view controller installs a standard gesture recognizer to drive the reordering process.

