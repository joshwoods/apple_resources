

- UIKit
-  UIContextMenuInteractionAnimating 

Protocol

# UIContextMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with context menus.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UIContextMenuInteractionAnimating : NSObjectProtocol
```

## Topics

### Adding Custom Animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

**Required**

func addCompletion(() -> Void)

Adds the specified completion block to the animator.

**Required**

### Previewing the Content

var previewViewController: UIViewController?

The current preview view controller.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIContextMenuInteractionCommitAnimating

## See Also

### Handling animations

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display begins.

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display ends.

