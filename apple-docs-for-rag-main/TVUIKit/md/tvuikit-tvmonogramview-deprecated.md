

- TVUIKit
-  TVMonogramView Deprecated

Class

# TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

tvOS 12.0+

``` source
@MainActor
class TVMonogramView
```

Deprecated

Use TVMonogramContentView instead.

## Overview

If you don’t provide an image, the system provides a generic placeholder image. If personNameComponents is not `nil`, the system creates a localized monogram image using the first initials from the name components.

## Topics

### Configuring a Monogram

var personNameComponents: PersonNameComponents?

The names used to create a monogram image.

var image: UIImage?

The custom image for the monogram.

var title: String?

The title for the monogram.

var subtitle: String?

The subtitle for the monogram.

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

class TVPosterView

An optimized view for displaying an image, a header, and a footer.

class TVCaptionButtonView

A button-like view that responds to user interactions.

