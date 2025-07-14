

- UIKit
- UICollectionViewDropProposal
-  UICollectionViewDropProposal.Intent 

Enumeration

# UICollectionViewDropProposal.Intent

Constants indicating how you intend to handle a drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Intent
```

## Topics

### Enumeration Cases

case insertAtDestinationIndexPath

Insert the dropped items at the specified index path.

case insertIntoDestinationIndexPath

Incorporate the dropped items into the item at the specified index path.

case unspecified

No drop proposal was specified.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Proposed Drop Location

var intent: UICollectionViewDropProposal.Intent

The option to use when incorporating the dropped items into your content.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

