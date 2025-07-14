

- UIKit
- UITableViewDropProposal
-  UITableViewDropProposal.Intent 

Enumeration

# UITableViewDropProposal.Intent

Constants indicating how you intend to handle a drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Intent
```

## Topics

### Constants

case unspecified

No drop proposal was specified.

case insertAtDestinationIndexPath

Insert the dropped content at the specified index path.

case insertIntoDestinationIndexPath

Incorporate the dropped content into the row at the specified index path.

case automatic

Incorporate the content in an appropriate way based on the drop location.

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

### Getting the proposed drop location

var intent: UITableViewDropProposal.Intent

The option to use when incorporating dropped items into your content.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

