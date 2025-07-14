

- UIKit
-  UITabBarItemAppearance 

Class

# UITabBarItemAppearance

An object for customizing the appearance of tab bar items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UITabBarItemAppearance
```

## Overview

Use a UITabBarItemAppearance object to customize the appearance of a tab bar item in each of its possible states. You can customize the appearance differently for each state. For example, you might apply different colors to the tab bar item’s icon in the normal and selected states.

## Topics

### Creating a tab bar item appearance object

init(style: UITabBarItemAppearance.Style)

Creates an appearance object with appropriate default values for a tab bar, displaying its items with the specified layout style.

convenience init()

Creates an appearance object with default values for a stacked tab bar item.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

### Copying a tab bar item appearance object

func copy() -> Self

Creates a copy of the appearance object.

### Resetting the appearance properties

func configureWithDefault(for: UITabBarItemAppearance.Style)

Configures the tab bar item appearance object with appropriate values for the specified style.

enum Style

Constants indicating the layout of a tab bar item’s content.

### Configuring attributes for different item states

var normal: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s enabled, unselected, and not the focused item.

var selected: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s selected.

var disabled: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s disabled.

var focused: UITabBarItemStateAppearance

The appearance data to apply to the tab bar item when it’s focused.

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

### Tab bar appearance

class UITabBarAppearance

An object for customizing the appearance of a tab bar.

class UITabBarItemStateAppearance

A data object containing the specific customizations for tab bar items in a particular state.

