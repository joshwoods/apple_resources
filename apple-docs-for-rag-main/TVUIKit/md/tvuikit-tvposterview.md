

- TVUIKit
-  TVPosterView 

Class

# TVPosterView

An optimized view for displaying an image, a header, and a footer.

tvOS 12.0+

``` source
@MainActor
class TVPosterView
```

## Overview

The `TVPosterView` object is a specialized TVLockupView used to display media items. The size of the poster view expands when it comes into focus.

## Topics

### Creating a Poster View

init(image: UIImage?)

Creates a new poster view using the supplied image.

### Configuring a Poster View

var image: UIImage?

The image for the poster view.

var imageView: UIImageView

The image view associated with the poster view.

var title: String?

The title for the poster view.

var subtitle: String?

The subtitle for the poster view.

## Relationships

### Inherits From

- TVLockupView

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
- UIContextMenuInteractionDelegate
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

### Lockup views

class TVLockupView

A focusable view that presents main content, like a movie poster, and an optional header and footer.

protocol TVLockupViewComponent

The protocol for responding to lockup view state changes.

class TVLockupHeaderFooterView

A view that contains header and footer information.

class TVCardView

A view that responds to focus interaction with a motion effect it applies to all of its subviews.

class TVCaptionButtonView

A button-like view that responds to user interactions.

class TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

Deprecated

