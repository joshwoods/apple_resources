

- UIKit
-  UIVibrancyEffect 

Class

# UIVibrancyEffect

An object that amplifies and adjusts the color of the content layered behind a visual effect view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIVibrancyEffect
```

## Overview

A vibrancy effect is intended to be used as a subview of or layered on top of a UIVisualEffectView that has been configured with a UIBlurEffect. The use of a vibrancy effect can help the content placed inside the contentView become more vivid.

The vibrancy effect is color-dependent. Any subviews that you add to the contentView must implement the tintColorDidChange() method and update themselves accordingly. UIImageView objects with images that have a rendering mode of UIImage.RenderingMode.alwaysTemplate as well as UILabel objects update automatically.

## Topics

### Creating a vibrancy effect

init(forBlurEffect: UIBlurEffect, style: UIVibrancyEffectStyle)

Creates a vibrancy effect with the specified blur and style values.

init(blurEffect: UIBlurEffect)

Creates a vibrancy effect for a specific blur effect.

enum UIVibrancyEffectStyle

Constants for the vibrancy styles.

### Deprecated

class func widgetPrimary() -> UIVibrancyEffect

Creates a vibrancy effect suitable for use with certain supporting text and template images within a widget.

Deprecated

class func widgetSecondary() -> UIVibrancyEffect

Creates a vibrancy effect suitable for indicating the secondary importance or relevance of supporting text and template images within a widget.

Deprecated

class func widgetEffect(forVibrancyStyle: UIVibrancyEffectStyle) -> UIVibrancyEffect

Creates a vibrancy effect for the specified style.

Deprecated

class func notificationCenter() -> UIVibrancyEffect

Creates a vibrancy effect for use in Notification Center.

Deprecated

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
- Sendable

## See Also

### Visual effects

class UIVisualEffect

An initializer for visual effect views and blur and vibrancy effect objects.

class UIVisualEffectView

An object that implements some complex visual effects.

class UIBlurEffect

An object that applies a blurring effect to the content layered behind a visual effect view.

