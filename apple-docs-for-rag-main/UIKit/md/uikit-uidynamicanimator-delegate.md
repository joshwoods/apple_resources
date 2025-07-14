

- UIKit
- UIDynamicAnimator
-  delegate 

Instance Property

# delegate

The delegate for responding to pausing or resumption of animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
weak var delegate: (any UIDynamicAnimatorDelegate)? { get set }
```

## Discussion

The methods for a dynamic animator delegate are described in UIDynamicAnimatorDelegate.

## See Also

### Responding to animation changes

protocol UIDynamicAnimatorDelegate

To respond to the pausing or resumption of UIKit dynamic animation, configure a custom class to adopt the UIDynamicAnimatorDelegate protocol. Then, in a dynamic animator (an instance of the UIDynamicAnimator class), set the delegate to be an instance of your custom class.

