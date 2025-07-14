

- UIKit
-  UINavigationBarAppearance 

Class

# UINavigationBarAppearance

An object for customizing the appearance of a navigation bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UINavigationBarAppearance
```

## Overview

After creating a UINavigationBarAppearance object, use the methods and properties of this class to specify the appearance you want for items in the navigation bar. Use the inherited properties from UIBarAppearance to configure the background and shadow attributes of the navigation bar itself.

## Topics

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of a standard-size title.

var largeTitleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of a large-size title.

var titlePositionAdjustment: UIOffset

The distance, in points, by which to offset the title horizontally and vertically.

### Configuring bar button items

var buttonAppearance: UIBarButtonItemAppearance

The appearance attributes for plain bar button items in the navigation bar.

### Configuring the Back button

var backButtonAppearance: UIBarButtonItemAppearance

The appearance attributes for the back button.

var backIndicatorImage: UIImage

The image to display on the leading edge of the back button.

var backIndicatorTransitionMaskImage: UIImage

The image for masking content flowing under the back indicator image during push and pop transitions.

func setBackIndicatorImage(UIImage?, transitionMaskImage: UIImage?)

Sets the back button indicator image and its transition mask.

### Configuring the Done button

var doneButtonAppearance: UIBarButtonItemAppearance

The appearance attributes for Done buttons.

## Relationships

### Inherits From

- UIBarAppearance

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

