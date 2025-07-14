

- UIKit
-  UIBlurEffect 

Class

# UIBlurEffect

An object that applies a blurring effect to the content layered behind a visual effect view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIBlurEffect
```

## Overview

Views that you add to the contentView of a visual effect view aren’t affected by the blur effect.

## Topics

### Creating a blur effect

init(style: UIBlurEffect.Style)

Creates a blur effect with the designated style.

### Constants

enum Style

Blur styles available for blur effect objects.

## Relationships

### Inherits From

- UIVisualEffect

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

## See Also

### Visual effects

class UIVisualEffect

An initializer for visual effect views and blur and vibrancy effect objects.

class UIVisualEffectView

An object that implements some complex visual effects.

class UIVibrancyEffect

An object that amplifies and adjusts the color of the content layered behind a visual effect view.

