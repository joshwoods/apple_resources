

- UIKit
- UICollectionViewDropCoordinator
-  proposal 

Instance Property

# proposal

The current proposal for how to incorporate the dropped items.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var proposal: UICollectionViewDropProposal { get }
```

**Required**

## Discussion

If your drag delegate implements the collectionView(_:dropSessionDidUpdate:withDestinationIndexPath:) method, this object contains the information that you provided when making your drop proposal for the given location.

## See Also

### Getting the Session Information

var session: any UIDropSession

The drop session containing information about the transaction.

**Required**

