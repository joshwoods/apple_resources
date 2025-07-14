

- UIKit
-  UIEditMenuInteractionDelegate 

Protocol

# UIEditMenuInteractionDelegate

The methods for customizing the menu the interaction displays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UIEditMenuInteractionDelegate : NSObjectProtocol
```

## Overview

You use this protocol to customize the actions or presentation of the menu an UIEditMenuInteraction object displays.

## Topics

### Customizing the Menu

func editMenuInteraction(UIEditMenuInteraction, menuFor: UIEditMenuConfiguration, suggestedActions: [UIMenuElement]) -> UIMenu?

Provides the menu to use when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, targetRectFor: UIEditMenuConfiguration) -> CGRect

Provides the target rectangle to position the menu relative to when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, willPresentMenuFor: UIEditMenuConfiguration, animator: any UIEditMenuInteractionAnimating)

Informs the delegate when the interaction is about to present the menu.

func editMenuInteraction(UIEditMenuInteraction, willDismissMenuFor: UIEditMenuConfiguration, animator: any UIEditMenuInteractionAnimating)

Informs the delegate when the interaction is about to dismiss the menu.

protocol UIEditMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with menus.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Edit menus

class UIEditMenuInteraction

An interaction that provides edit operations using a menu.

class UIEditMenuConfiguration

An object containing the configuration details for the menu your app presents in response to an edit menu interaction.

protocol UIResponderStandardEditActions

A set of standard methods that apps can adopt to support editing.

