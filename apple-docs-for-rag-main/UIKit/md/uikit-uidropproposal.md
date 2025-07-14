

- UIKit
-  UIDropProposal 

Class

# UIDropProposal

A configuration for the behavior of a drop interaction, required if a view accepts drop activities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIDropProposal
```

## Mentioned in 

Making a view into a drop destination

## Overview

If a view’s drop interaction delegate accepts dropped drag items, it must return a drop proposal in its implementation of the dropInteraction(_:sessionDidUpdate:) method.

## Topics

### Initializing a drop proposal

init(operation: UIDropOperation)

Initializes a new drop proposal with a drop operation type.

var operation: UIDropOperation

The drop operation that the drop interaction proposes to perform.

### Configuring a drop proposal

var isPrecise: Bool

A Boolean value that proposes that the drop interaction define the drop location precisely, such as at a specific point within existing text.

var prefersFullSizePreview: Bool

A Boolean value that indicates that the drag item preview should be shown at its full, original size.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UICollectionViewDropProposal
- UITableViewDropProposal
- UITextDropProposal

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Drop destinations

protocol UIDropSession

The interface for querying a drop session about its state and associated drag items.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

enum UIDropSessionProgressIndicatorStyle

The drop-progress indicator styles for the drop session, used while data is moving from the source to the destination.

