

- UIKit
-  UIViewImplicitlyAnimating 

Protocol

# UIViewImplicitlyAnimating

An interface for modifying an animation while it’s running.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIViewImplicitlyAnimating : UIViewAnimating
```

## Overview

Animator objects used in interruptible view controller transitions adopt the UIViewImplicitlyAnimating protocol to modify in-flight transition animations. This protocol also conforms to the UIViewAnimating protocol, which specifies methods for starting and stopping animations and for updating their state.

The UIViewPropertyAnimator class adopts this protocol and implements all of its methods. You can adopt this protocol in your own classes to implement custom animator objects. When adopting this protocol, it’s recommended that you implement all of the methods.

## Topics

### Modifying animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block to the animator with a delay.

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds the specified completion block to the animator.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the final timing and duration of a paused animation.

## Relationships

### Inherits From

- NSObjectProtocol
- UIViewAnimating

### Conforming Types

- UIViewPropertyAnimator

