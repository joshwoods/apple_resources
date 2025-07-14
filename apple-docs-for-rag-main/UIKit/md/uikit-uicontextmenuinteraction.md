

- UIKit
-  UIContextMenuInteraction 

Class

# UIContextMenuInteraction

An interaction object that you use to display relevant actions for your content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UIContextMenuInteraction
```

## Mentioned in 

Building a desktop-class iPad app

## Overview

Use a UIContextMenuInteraction object to focus the user’s attention on a specific portion of your content, and to provide actions for the user to perform on that content. A context menu interaction object tracks Force Touch gestures on devices that support 3D Touch, and long-press gestures on devices that don’t support it. When the appropriate gesture occurs, this object animates your content to a new interface and displays the contextual menu that you supplied. UIKit manages all menu-related interactions and reports the selected action, if any, back to your app.

A context menu interaction object inherits from UIInteraction. After creating the object, assign an appropriate object to its delegate property and use the addInteraction(_:) method to attach it to one of your views. The delegate object you provide must adopt the UIContextMenuInteractionDelegate protocol. Use the methods of that object to provide the contents of the contextual menu. Add your context menu interaction object to a view in your interface using the view’s addInteraction(_:) method.

## Topics

### Creating a context menu interaction object

init(delegate: any UIContextMenuInteractionDelegate)

Creates a context menu interaction object with the specified delegate object.

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

### Previewing and managing the content

var delegate: (any UIContextMenuInteractionDelegate)?

The object that provides the preview and contextual menu for your content and responds to interaction-related events.

protocol UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

### Getting the interaction’s location

func location(in: UIView?) -> CGPoint

Returns the location of the user interaction in the specified view’s coordinate system.

### Getting the menu appearance

var menuAppearance: UIContextMenuInteraction.appearance

The appearance of the context menu.

enum appearance

Constants that describe the appearance of the menu.

### Managing menu interactions

func dismissMenu()

Dismisses the context menu.

func updateVisibleMenu((UIMenu) -> UIMenu)

Updates the currently visible menu.

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
- UIInteraction

## See Also

### Contextual menus

protocol UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

class UITargetedPreview

An object describing the view to use during preview-related animations.

class UIPreviewTarget

An object that specifies the container view to use for animations.

class UIPreviewParameters

Additional parameters to use when animating a preview interface.

