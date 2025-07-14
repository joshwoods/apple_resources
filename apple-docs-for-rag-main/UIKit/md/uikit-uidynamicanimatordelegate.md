

- UIKit
-  UIDynamicAnimatorDelegate 

Protocol

# UIDynamicAnimatorDelegate

To respond to the pausing or resumption of UIKit dynamic animation, configure a custom class to adopt the UIDynamicAnimatorDelegate protocol. Then, in a dynamic animator (an instance of the UIDynamicAnimator class), set the delegate to be an instance of your custom class.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIDynamicAnimatorDelegate : NSObjectProtocol
```

## Topics

### Responding to animation pausing and resumption

func dynamicAnimatorDidPause(UIDynamicAnimator)

Called when a dynamic animator pauses the animations for its behaviors’ associated dynamic items.

func dynamicAnimatorWillResume(UIDynamicAnimator)

Called when a dynamic animator is about to resume the animations for its behaviors’ associated dynamic items.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to animation changes

var delegate: (any UIDynamicAnimatorDelegate)?

The delegate for responding to pausing or resumption of animation.

