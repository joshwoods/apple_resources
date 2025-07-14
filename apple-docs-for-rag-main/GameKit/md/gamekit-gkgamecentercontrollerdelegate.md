

- GameKit
-  GKGameCenterControllerDelegate 

Protocol

# GKGameCenterControllerDelegate

The delegate that GameKit calls when the player dismisses the dashboard.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
protocol GKGameCenterControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Displaying the Game Center dashboard

## Overview

Delegates of GKGameCenterViewController objects conform to the `GKGameCenterControllerDelegate` protocol.

## Topics

### Handling User Actions

func gameCenterViewControllerDidFinish(GKGameCenterViewController)

Handles when the player dismisses the dashboard.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the view controller delegate

var gameCenterDelegate: (any GKGameCenterControllerDelegate)?

The view controller’s delegate.

