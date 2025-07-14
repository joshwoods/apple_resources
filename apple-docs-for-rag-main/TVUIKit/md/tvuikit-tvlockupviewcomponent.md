

- TVUIKit
-  TVLockupViewComponent 

Protocol

# TVLockupViewComponent

The protocol for responding to lockup view state changes.

tvOS 12.0+

``` source
protocol TVLockupViewComponent : NSObjectProtocol
```

## Topics

### Updating the Lockup View Appearance

func updateAppearance(forLockupViewState: UIControl.State)

Provides an opportunity to change the appearance of a view when a state changes.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- TVLockupHeaderFooterView

## See Also

### Lockup views

class TVLockupView

A focusable view that presents main content, like a movie poster, and an optional header and footer.

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

