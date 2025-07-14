

- TVUIKit
-  TVCollectionViewFullScreenLayoutAttributes 

Class

# TVCollectionViewFullScreenLayoutAttributes

Attributes to manage the appearance of the collection view’s layout.

tvOS 13.0+

``` source
@MainActor
class TVCollectionViewFullScreenLayoutAttributes
```

## Topics

### Modifying Cell Appearance

var contentBleed: UIEdgeInsets

The amount of content that bleeds into the masked portions of the cell.

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the cell.

var maskAmount: CGFloat

The amount of masking to apply to the cell.

### Modifying the Parallax Effect

var parallaxOffset: CGFloat

The number of points by which to shift the background from the center when moving focus.

### Managing Cell Position

var normalizedPosition: CGFloat

A value that indicates the distance of the current cell from the collection view’s center cell.

## Relationships

### Inherits From

- UICollectionViewLayoutAttributes

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- UIDynamicItem

## See Also

### Collections of content

Creating immersive experiences using a full-screen layout

Display content with a collection view that maximizes the tvOS experience.

class TVCollectionViewFullScreenLayout

A collection view layout that organizes items into a browsable, full-screen display format.

protocol TVCollectionViewDelegateFullScreenLayout

Methods that send notifications of events during cell transitions.

class TVCollectionViewFullScreenCell

A full-screen cell to use in full-screen display format.

