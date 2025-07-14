

- UIKit
- UIBlurEffect
-  UIBlurEffect.Style 

Enumeration

# UIBlurEffect.Style

Blur styles available for blur effect objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum Style
```

## Topics

### Adaptable styles

case systemUltraThinMaterial

An adaptable blur effect that creates the appearance of an ultra-thin material.

case systemThinMaterial

An adaptable blur effect that creates the appearance of a thin material.

case systemMaterial

An adaptable blur effect that creates the appearance of a material with normal thickness.

case systemThickMaterial

An adaptable blur effect that creates the appearance of a material that’s thicker than normal.

case systemChromeMaterial

An adaptable blur effect that creates the appearance of the system chrome.

### Light styles

case systemUltraThinMaterialLight

A blur effect that creates the appearance of an ultra-thin material and is always light.

case systemThinMaterialLight

A blur effect that creates the appearance of a thin material and is always light.

case systemMaterialLight

A blur effect that creates the appearance of a material with normal thickness and is always light.

case systemThickMaterialLight

A blur effect that creates the appearance of a material that’s thicker than normal and is always light.

case systemChromeMaterialLight

A blur effect that creates the appearance of the system chrome and is always light.

### Dark styles

case systemUltraThinMaterialDark

A blur effect that creates the appearance of an ultra-thin material and is always dark.

case systemThinMaterialDark

A blur effect that creates the appearance of a thin material and is always dark.

case systemMaterialDark

A blur effect that creates the appearance of a material with normal thickness and is always dark.

case systemThickMaterialDark

A blur effect that creates the appearance of a material that’s thicker than normal and is always dark.

case systemChromeMaterialDark

A blur effect that creates the appearance of the system chrome and is always dark.

### Additional styles

case extraLight

The area of the view is lighter than the underlying view.

case light

The area of the view is the same approximate lightness of the underlying view.

case dark

The area of the view is darker than the underlying view.

case extraDark

The area of the view is even more dark than the underlying view.

case regular

A regular blur style that adapts to the user interface style.

case prominent

A blur style for making content more prominent that adapts to the user interface style.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

