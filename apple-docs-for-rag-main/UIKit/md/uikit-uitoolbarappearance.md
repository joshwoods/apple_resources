

- UIKit
-  UIToolbarAppearance 

Class

# UIToolbarAppearance

An object for customizing the appearance of a toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIToolbarAppearance
```

## Overview

After creating a UIToolbarAppearance object, use the methods and properties of this class to specify the appearance of items in the toolbar. Use the inherited properties from UIBarAppearance to configure the background and shadow attributes of the toolbar itself.

## Topics

### Configuring bar button items

var buttonAppearance: UIBarButtonItemAppearance

The appearance attributes for plain bar button items in the toolbar.

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

