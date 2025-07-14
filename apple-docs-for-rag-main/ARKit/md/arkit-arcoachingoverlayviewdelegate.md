

- ARKit
-  ARCoachingOverlayViewDelegate 

Protocol

# ARCoachingOverlayViewDelegate

A set of callbacks you implement to be notified of coaching events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
protocol ARCoachingOverlayViewDelegate : NSObjectProtocol
```

## Overview

Implement a delegate to coordinate your app’s actions with coaching overlay. For example, when the coaching overlay determines the user needs guidance, you hide your app’s UI to allow the user to focus on the coaching experience. When the coaching overlay determines the goal is met, you show your app’s UI and begin your app’s AR experience.

## Topics

### Enabling Coaching

func coachingOverlayViewWillActivate(ARCoachingOverlayView)

Tells you when the coaching overlay view activates.

func coachingOverlayViewDidDeactivate(ARCoachingOverlayView)

Tells you when the coaching experience is completely deactivated.

### Restarting the Session

func coachingOverlayViewDidRequestSessionReset(ARCoachingOverlayView)

Tells you when the user taps the coaching overlay view’s Start Over button while the session is relocalizing.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Delegating Events

var delegate: (any ARCoachingOverlayViewDelegate)?

An object you supply that implements coaching event callbacks.

