

- TVUIKit
-  TVLockupView 

Class

# TVLockupView

A focusable view that presents main content, like a movie poster, and an optional header and footer.

tvOS 12.0+

``` source
@MainActor
class TVLockupView
```

## Overview

A `TVLockupView` object consists of three views that operate as a single view. The content view typically contains a media item image, like a movie poster, with additional information in the header and footer views. The `TVLockupView` object expands when it comes into focus, using focusSizeIncrease and contentSize to calculate the size increase. Provide sufficient `focusSizeIncrease` values so that your custom content doesn’t overlap other objects when the content comes into focus.

The following figure shows a `TVLockupView` object that’s in focus. The yellow, vertical bars indicate the space between views. The center view is in focus and has increased in size, expanding into the space between views. Views don’t move as other views come into focus.

Note

Don’t create a TVLockupView directly. Instead, create an instance of the subclass that best suits your use case, such as TVPosterView or TVCardView.

## Topics

### Setting view size

var contentSize: CGSize

The size of the content view.

var contentViewInsets: NSDirectionalEdgeInsets

The spacing between the content view and its peer and containing views.

var focusSizeIncrease: NSDirectionalEdgeInsets

The inset or outset values specifying your content’s size increase when in focus.

### Adding subviews

var contentView: UIView

The main view for the lockup.

var headerView: TVLockupHeaderFooterView?

A view containing header information.

var footerView: TVLockupHeaderFooterView?

A view containing footer information.

## Relationships

### Inherits From

- UIControl

### Inherited By

- TVCaptionButtonView
- TVCardView
- TVMonogramView
- TVPosterView

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

class TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

Deprecated

