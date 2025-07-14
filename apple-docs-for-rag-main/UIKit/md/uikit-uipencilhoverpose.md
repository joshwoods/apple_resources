

- UIKit
-  UIPencilHoverPose 

Class

# UIPencilHoverPose

An object that describes the hover pose of Apple Pencil during an interaction like double tap or squeeze.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
class UIPencilHoverPose
```

## Overview

Use the hover pose of Apple Pencil to support more complex interactions in response to a double tap or squeeze. Information about the hover pose — such as azimuth, altitude, and hover distance — is available when a person holds a supported model of Apple Pencil close to the screen during a double tap or squeeze.

The following code example shows how to use the location of a hover pose to present a contextual palette near the tip of Apple Pencil.

```
func pencilInteraction(_ interaction: UIPencilInteraction,
                       didReceiveSqueeze squeeze: UIPencilInteraction.Squeeze) {
    let preferredAction = UIPencilInteraction.preferredSqueezeAction

    if preferredAction == .showContextualPalette, squeeze.phase == .ended {
        if let anchorPoint = squeeze.hoverPose?.location {
            presentContextualPalette(atLocation: anchorPoint)
        }
    }
}
```

## Topics

### Getting the hover characteristics

var location: CGPoint

The location of an Apple Pencil above the view’s bounds, in view’s coordinate space.

var altitudeAngle: CGFloat

A value that represents the altitude angle of Apple Pencil.

var azimuthAngle: CGFloat

A value that represents the azimuth angle of Apple Pencil.

var azimuthUnitVector: CGVector

A value that represents the azimuth unit vector of Apple Pencil in the specified view.

var rollAngle: CGFloat

A value that represents the barrel-roll angle of Apple Pencil.

var zOffset: CGFloat

A value that represents the normalized distance between the screen and Apple Pencil.

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

### Apple Pencil interactions in UIKit

class UIPencilInteraction

An interaction that tells your app when a person double-taps or squeezes Apple Pencil.

protocol UIPencilInteractionDelegate

The interface an object implements to handle double taps or squeezes a person makes on Apple Pencil.

class Tap

An interaction that represents a double tap on Apple Pencil.

class Squeeze

An interaction that represents a squeeze on Apple Pencil.

enum Phase

Constants that describe the phases of an interaction on Apple Pencil.

