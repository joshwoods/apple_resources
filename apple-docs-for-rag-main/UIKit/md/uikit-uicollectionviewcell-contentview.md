

- UIKit
- UICollectionViewCell
-  contentView 

Instance Property

# contentView

The main view that you add your cell’s custom content to.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentView: UIView { get }
```

## Discussion

When configuring a cell, you add any custom views representing your cell’s content to this view. The cell object places the content in this view in front of any background views.

## See Also

### Managing the content

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the cell.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its content configuration when its state changes.

