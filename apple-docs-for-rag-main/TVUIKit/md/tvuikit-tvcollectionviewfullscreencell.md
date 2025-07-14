

- TVUIKit
-  TVCollectionViewFullScreenCell 

Class

# TVCollectionViewFullScreenCell

A full-screen cell to use in full-screen display format.

tvOS 13.0+

``` source
@MainActor
class TVCollectionViewFullScreenCell
```

## Overview

Use `TVCollectionViewFullScreenCell` to populate the full-screen collection view with content.

## Topics

### Modifying Cell Appearance

var contentBleed: UIEdgeInsets

The amount of content that overlaps into the masked portions of the cell.

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the cell.

var maskAmount: CGFloat

The factor that determines the amount of masking applied on the cell.

### Accessing Cell Views

var maskedContentView: UIView

The content view in focus.

var maskedBackgroundView: UIView

The background view that performs the parallax effect.

### Accessing Cell Position

var normalizedPosition: CGFloat

The value that determines the current cell’s relative position on the screen.

### Managing Cell Position

func normalizedPositionDidChange()

Notifies the cell when its normalized position changes.

func normalizedPositionWillChange(CGFloat)

Notifies the cell when its normalized position is about to change.

### Managing Cell Mask

func maskAmountDidChange()

Notifies the cell when its mask amount changes.

func maskAmountWillChange(CGFloat)

Notifies the cell when its mask amount is about to change.

### Managing the Parallax Effect

var parallaxOffset: CGFloat

The number of pixels by which to shift the background from the center when moving focus.

## Relationships

### Inherits From

- UICollectionViewCell

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIAccessibilityIdentification
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Collections of content

Creating immersive experiences using a full-screen layout

Display content with a collection view that maximizes the tvOS experience.

class TVCollectionViewFullScreenLayout

A collection view layout that organizes items into a browsable, full-screen display format.

protocol TVCollectionViewDelegateFullScreenLayout

Methods that send notifications of events during cell transitions.

class TVCollectionViewFullScreenLayoutAttributes

Attributes to manage the appearance of the collection view’s layout.

