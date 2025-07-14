

- UIKit
-  UIBarButtonItemAppearance 

Class

# UIBarButtonItemAppearance

An object for customizing the appearance of bar button items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIBarButtonItemAppearance
```

## Overview

Use a UIBarButtonItemAppearance object to customize the appearance of a bar button item in each of its possible states. You can customize the appearance differently for different states. For example, you might apply different colors to the button’s title in the normal and highlighted states.

## Topics

### Creating a bar button item appearance object

init(style: UIBarButtonItem.Style)

Creates an appearance with default values that are appropriate for the specified button style.

convenience init()

Creates an appearance object with default values that are appropriate for a plain button.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

### Copying a bar button item bar appearance object

func copy() -> Self

Creates a copy of the appearance object.

### Resetting the appearance properties

func configureWithDefault(for: UIBarButtonItem.Style)

Configures the bar button item appearance object with appropriate values for the specified button style.

### Configuring attributes for different button states

var normal: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the normal state.

var disabled: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the disabled state.

var highlighted: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s in the highlighted state.

var focused: UIBarButtonItemStateAppearance

The appearance data to apply to the button when it’s focused.

## Relationships

### Inherits From

- NSObject

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

### Shared appearance

class UIBarAppearance

An object for customizing the basic appearance of system bars.

class UIBarButtonItemStateAppearance

A data object containing the specific customizations for a bar button item in a particular state.

