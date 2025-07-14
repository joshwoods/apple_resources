

- UIKit
-  UIEditMenuConfiguration 

Class

# UIEditMenuConfiguration

An object containing the configuration details for the menu your app presents in response to an edit menu interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UIEditMenuConfiguration
```

## Overview

You use this object when calling the presentEditMenu(with:) method of UIEditMenuInteraction to provide the configuration details the interaction’s delegate uses to construct the menu that the interaction displays.

## Topics

### Creating an edit menu configuration

convenience init(identifier: AnyHashable?, sourcePoint: CGPoint)

Initializes a new configuration with the source location you specify.

### Getting the configuration identifier

var identifier: AnyHashable

The unique identifier for this configuration object.

### Configuring the menu

var preferredArrowDirection: UIEditMenuArrowDirection

The preferred direction the arrow of the edit menu is pointing.

enum UIEditMenuArrowDirection

Constants that describe the direction the arrow of the edit menu is pointing.

var sourcePoint: CGPoint

The source location of the interaction.

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

### Edit menus

class UIEditMenuInteraction

An interaction that provides edit operations using a menu.

protocol UIEditMenuInteractionDelegate

The methods for customizing the menu the interaction displays.

protocol UIResponderStandardEditActions

A set of standard methods that apps can adopt to support editing.

