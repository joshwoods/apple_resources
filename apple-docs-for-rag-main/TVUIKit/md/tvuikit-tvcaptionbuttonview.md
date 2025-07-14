

- TVUIKit
-  TVCaptionButtonView 

Class

# TVCaptionButtonView

A button-like view that responds to user interactions.

tvOS 12.0+

``` source
@MainActor
class TVCaptionButtonView
```

## Overview

A caption button responds to user interactions and can contain an image or text. When the caption button comes into focus, the caption button expands in the leading, top, and trailing directions. The user can click the caption button to select an option. As the user moves their finger on the Siri Remote up and down, or left and right, the caption button may limit the direction of the tilt based on the type set in motionDirection.

## Topics

### Setting the Motion Direction

var motionDirection: TVCaptionButtonViewMotionDirection

The direction that the caption button view tilts in response to user interaction on the remote.

enum TVCaptionButtonViewMotionDirection

The directions that the caption button view can tilt in response to user interactions on the remote.

### Configuring the Caption Button

var contentImage: UIImage?

The image displayed in the main content view.

var contentText: String?

The text displayed in the main content view.

var title: String?

The title for the caption button.

var subtitle: String?

The subtitle of the caption button.

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

class TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

Deprecated

