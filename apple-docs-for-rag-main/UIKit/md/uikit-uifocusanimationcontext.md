

- UIKit
-  UIFocusAnimationContext 

Protocol

# UIFocusAnimationContext

Information about focusing animations being performed by the system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
protocol UIFocusAnimationContext : NSObjectProtocol
```

## Overview

You don’t adopt this protocol in your custom classes. When a focus update occurs and the system provides you with a UIFocusAnimationCoordinator object, you can use that object to specify custom focus-related animations. When the time comes for the system to execute your animations, it delivers an object that adopts this protocol to your animation block. The context object contains information about the system animations that you can use to configure the behavior of your own animations. For example, you might configure your animations to be exactly half the duration of the system animations.

## Topics

### Getting the animation attributes

var duration: TimeInterval

The duration (measured in seconds) of the focus animation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Adding animations to focus updates

func addCoordinatedFocusingAnimations(((any UIFocusAnimationContext) -> Void)?, completion: (() -> Void)?)

Runs the specified set of animations together with the system animations for adding focus to an item.

func addCoordinatedUnfocusingAnimations(((any UIFocusAnimationContext) -> Void)?, completion: (() -> Void)?)

Runs the specified set of animations together with the system animations for removing focus from an item.

func addCoordinatedAnimations((() -> Void)?, completion: (() -> Void)?)

Specifies the animations to coordinate with the active focus animation.

