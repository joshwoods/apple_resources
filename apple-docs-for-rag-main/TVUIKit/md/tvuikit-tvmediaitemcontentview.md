

- TVUIKit
-  TVMediaItemContentView 

Class

# TVMediaItemContentView

A view that represents media content, such as movies and TV shows.

tvOS 15.0+

``` source
@MainActor
class TVMediaItemContentView
```

## Overview

The following code illustrates how to update the configuration for a wide media item:

```
```

## Topics

### Creating a Media Item Content View

convenience init(configuration: TVMediaItemContentConfiguration)

Creates a media item content view with the configuration you specify.

struct TVMediaItemContentConfiguration

A content configuration for a media item view.

### Managing the Content Layout

var focusedFrameGuide: UILayoutGuide

A guide for positioning other elements with the content view image’s focused frame.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
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
- UIContentView
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

### Content views

class TVMonogramContentView

A view that contains a circular image of a person or the person’s initials.

