

- TVUIKit
-  TVLockupHeaderFooterView 

Class

# TVLockupHeaderFooterView

A view that contains header and footer information.

tvOS 12.0+

``` source
@MainActor
class TVLockupHeaderFooterView
```

## Overview

You can add header and footer views containing titles and subtitles to the lockup view. Headers and footers are always displayed when the lockup view is in focus.

## Topics

### Adding Titles

var titleLabel: UILabel?

The title for a header or footer.

var subtitleLabel: UILabel?

The subtitle for a header or footer.

### Configuring Focus Behavior

var showsOnlyWhenAncestorFocused: Bool

A Boolean value indicating whether titles and subtitles are displayed when a lockup view isn’t in focus.

## Relationships

### Inherits From

- UIView

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
- TVLockupViewComponent
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

### Lockup views

class TVLockupView

A focusable view that presents main content, like a movie poster, and an optional header and footer.

protocol TVLockupViewComponent

The protocol for responding to lockup view state changes.

class TVCardView

A view that responds to focus interaction with a motion effect it applies to all of its subviews.

class TVPosterView

An optimized view for displaying an image, a header, and a footer.

class TVCaptionButtonView

A button-like view that responds to user interactions.

class TVMonogramView

A specialized lockup view that contains a circular image of a person or the person’s initials, along with a footer view.

Deprecated

