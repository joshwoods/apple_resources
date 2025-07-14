

- UIKit
-  UIBarButtonItemStateAppearance 

Class

# UIBarButtonItemStateAppearance

A data object containing the specific customizations for a bar button item in a particular state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIBarButtonItemStateAppearance
```

## Overview

Use a UIBarButtonItemStateAppearance object to customize the title and background image of your bar button items. Don’t create UIBarButtonItemStateAppearance objects yourself. Instead, create a UIBarButtonItemAppearance object and use its properties to fetch the appearance attributes for the button in a particular state. For example, to set the button’s attributes when it’s in the normal state, configure the object in the normal property.

## Topics

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of the bar button item’s title.

var titlePositionAdjustment: UIOffset

The additional amount by which to offset the title horizontally and vertically.

### Configuring the background appearance

var backgroundImage: UIImage?

A background image to display around the button.

var backgroundImagePositionAdjustment: UIOffset

The distance, in points, by which to offset the background image horizontally and vertically.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Shared appearance

class UIBarAppearance

An object for customizing the basic appearance of system bars.

class UIBarButtonItemAppearance

An object for customizing the appearance of bar button items.

