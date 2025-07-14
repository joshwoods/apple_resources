

- TVUIKit
-  TVCardView 

Class

# TVCardView

A view that responds to focus interaction with a motion effect it applies to all of its subviews.

tvOS 12.0+

``` source
@MainActor
class TVCardView
```

## Overview

A `TVCardView` object is a specialized version of TVLockupView that presents an arbitrarily composed view hierarchy in a floating content view. You add custom subviews to the contentView property, and the subviews act as a single unit in regard to selection and motion effects. You typically use a TVCardView to display ratings and reviews for a media item. The following figure shows a rating card that consists of two label views (the rating and related information) and an image view (the stars).

## Topics

### Setting the Background Color

var cardBackgroundColor: UIColor?

The background color of the content view.

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

class TVPosterView

An optimized view for displaying an image, a header, and a footer.

class TVCaptionButtonView

A button-like view that responds to user interactions.

class TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

Deprecated

