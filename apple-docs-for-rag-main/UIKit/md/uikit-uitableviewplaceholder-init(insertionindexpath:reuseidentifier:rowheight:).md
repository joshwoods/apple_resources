

- UIKit
- UITableViewPlaceholder
-  init(insertionIndexPath:reuseIdentifier:rowHeight:) 

Initializer

# init(insertionIndexPath:reuseIdentifier:rowHeight:)

Creates a placeholder object with the specified index path and cell-related information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    insertionIndexPath: IndexPath,
    reuseIdentifier: String,
    rowHeight: CGFloat
)
```

## Parameters 

`insertionIndexPath`  

The index path at which to insert the placeholder cell.

`reuseIdentifier`  

The reuse identifier to use when dequeueing the cell. A cell with the specified identifier must be registered with the table prior to inserting the placeholder cell. You can register cells in your storyboard file or programmatically.

`rowHeight`  

The initial height of the cell. Specify automaticDimension if your table uses estimated row heights and the placeholder cell is self-sizing.

## Return Value

A new placeholder cell object.

