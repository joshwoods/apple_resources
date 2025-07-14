

- UIKit
-  UIContextMenuInteractionDelegate 

Protocol

# UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UIContextMenuInteractionDelegate : NSObjectProtocol
```

## Mentioned in 

Building a desktop-class iPad app

## Overview

Use this protocol to provide UIKit with the contextual menu that you want to display. When a UIContextMenuInteraction object detects an appropriate interaction, it calls the contextMenuInteraction(_:configurationForMenuAtLocation:) method of your delegate. You use that method to specify the basic configuration details for your interface. In addition to your contextual menu, you can tell UIKit whether you want it to display a default preview interface or a custom view controller that you provide. You can also specify options for how you want UIKit to animate the presentation and dismissal of that interface.

For additional information about how to implement contextual menus, see Adding context menus in your app.

## Topics

### Providing the preview configuration data

func contextMenuInteraction(UIContextMenuInteraction, configurationForMenuAtLocation: CGPoint) -> UIContextMenuConfiguration?

Returns the configuration data to use when previewing the content.

**Required**

class UIContextMenuConfiguration

An object containing the configuration details for the contextual menu.

### Customizing the preview animations

func contextMenuInteraction(UIContextMenuInteraction, configuration: UIContextMenuConfiguration, highlightPreviewForItemWithIdentifier: any NSCopying) -> UITargetedPreview?

Asks the delegate for a preview of the item with the specified identifier when a context-menu interaction begins.

func contextMenuInteraction(UIContextMenuInteraction, configuration: UIContextMenuConfiguration, dismissalPreviewForItemWithIdentifier: any NSCopying) -> UITargetedPreview?

Asks the delegate for a preview of the item with the specified identifier when a context-menu interaction ends.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

### Responding to the menu’s appearance

func contextMenuInteraction(UIContextMenuInteraction, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a preview action begins.

protocol UIContextMenuInteractionCommitAnimating

Methods adopted by system-supplied animator objects when committing preview-related animations.

### Handling animations

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display begins.

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display ends.

protocol UIContextMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with context menus.

### Deprecated

func contextMenuInteraction(UIContextMenuInteraction, previewForHighlightingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the source view to use when animating the appearance of the preview interface.

Deprecated

func contextMenuInteraction(UIContextMenuInteraction, previewForDismissingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

Returns the destination view to use when animating the appearance of the preview interface.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIButton
- UIColorWell
- UIControl
- UIDatePicker
- UIPageControl
- UIPasteControl
- UIRefreshControl
- UISearchTextField
- UISegmentedControl
- UISlider
- UIStepper
- UISwitch
- UITextField

## See Also

### Contextual menus

class UIContextMenuInteraction

An interaction object that you use to display relevant actions for your content.

class UITargetedPreview

An object describing the view to use during preview-related animations.

class UIPreviewTarget

An object that specifies the container view to use for animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

