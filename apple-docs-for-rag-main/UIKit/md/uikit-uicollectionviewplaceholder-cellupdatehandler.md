

- UIKit
- UICollectionViewPlaceholder
-  cellUpdateHandler 

Instance Property

# cellUpdateHandler

The block that updates the contents of the placeholder cell.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var cellUpdateHandler: ((UICollectionViewCell) -> Void)? { get set }
```

## Discussion

Specify a block that configures or updates the appearance of your placeholder cell. The collection view calls this block when the placeholder cell becomes visible, and at other appropriate times.

