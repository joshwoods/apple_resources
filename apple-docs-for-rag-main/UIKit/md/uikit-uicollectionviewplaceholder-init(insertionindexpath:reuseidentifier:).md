

- UIKit
- UICollectionViewPlaceholder
-  init(insertionIndexPath:reuseIdentifier:) 

Initializer

# init(insertionIndexPath:reuseIdentifier:)

Creates a placeholder object with the specified index path and reuse identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    insertionIndexPath: IndexPath,
    reuseIdentifier: String
)
```

## Parameters 

`insertionIndexPath`  

The index path at which to insert the placeholder cell.

`reuseIdentifier`  

The reuse identifier to use when dequeueing the cell.

## Return Value

A new placeholder cell object.

