

- TVUIKit
-  TVMonogramContentView 

Class

# TVMonogramContentView

A view that contains a circular image of a person or the person’s initials.

tvOS 15.0+

``` source
@MainActor
class TVMonogramContentView
```

## Overview

The system provides a generic placeholder image if image is `nil`. If personNameComponents isn’t `nil`, the system creates a localized monogram image using the first initials from the name components.

The following code illustrates how to update the configuration for a monogram:

```
override func updateConfiguration(using state: UICellConfigurationState) {
    var configuration = TVMonogramContentConfiguration().updatedConfiguration(for: state)

    configuration.image = avatarImage
    configuration.text = "Anne Johnson"
    configuration.secondaryText = "Actor"
    configuration.personNameComponents = nameComponents

    self.contentConfiguration = configuration
}
```

## Topics

### Creating a Monogram Content View

convenience init(configuration: TVMonogramContentConfiguration)

Creates a monogram content view with the configuration you specify.

struct TVMonogramContentConfiguration

A content configuration for a monogram view.

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

class TVMediaItemContentView

A view that represents media content, such as movies and TV shows.

