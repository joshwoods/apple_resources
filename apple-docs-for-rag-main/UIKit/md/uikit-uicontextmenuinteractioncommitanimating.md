

- UIKit
-  UIContextMenuInteractionCommitAnimating 

Protocol

# UIContextMenuInteractionCommitAnimating

Methods adopted by system-supplied animator objects when committing preview-related animations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIContextMenuInteractionCommitAnimating : UIContextMenuInteractionAnimating
```

## Overview

When the user taps in a preview interface to dismiss it, UIKit creates an object that adopts this protocol and passes it to your UIContextMenuInteractionDelegate method. Use the object to add any custom animations that you want to run alongside the dismissal animations.

## Topics

### Specifying the Commit Style

var preferredCommitStyle: UIContextMenuInteractionCommitStyle

The preferred animation style triggered when the user taps the preview.

**Required**

enum UIContextMenuInteractionCommitStyle

Constants that control the interaction commit style.

## Relationships

### Inherits From

- NSObjectProtocol
- UIContextMenuInteractionAnimating

## See Also

### Responding to the menu’s appearance

func contextMenuInteraction(UIContextMenuInteraction, willPerformPreviewActionForMenuWith: UIContextMenuConfiguration, animator: any UIContextMenuInteractionCommitAnimating)

Informs the delegate when a preview action begins.

