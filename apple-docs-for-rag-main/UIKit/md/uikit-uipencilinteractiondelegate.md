

- UIKit
-  UIPencilInteractionDelegate 

Protocol

# UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+

``` source
@MainActor
protocol UIPencilInteractionDelegate : NSObjectProtocol
```

## Topics

### Handling double-tap interactions

func pencilInteraction(UIPencilInteraction, didReceiveTap: UIPencilInteraction.Tap)

Tells the delegate when a person double-taps Apple Pencil.

### Handling squeeze interactions

func pencilInteraction(UIPencilInteraction, didReceiveSqueeze: UIPencilInteraction.Squeeze)

Tells the delegate when a person squeezes Apple Pencil.

### Deprecated

func pencilInteractionDidTap(UIPencilInteraction)

Tells the delegate that the user double-tapped Apple Pencil.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Apple Pencil interactions in UIKit

class UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

class UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

