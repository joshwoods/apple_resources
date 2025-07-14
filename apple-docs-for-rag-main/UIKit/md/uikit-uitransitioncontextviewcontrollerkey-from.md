

- UIKit
- UITransitionContextViewControllerKey
-  from 

Type Property

# from

A key that identifies the view controller that’s visible at the beginning of the transition, or at the end of a canceled transition.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let from: UITransitionContextViewControllerKey
```

## Discussion

This view controller is typically the one presenting the “to” view controller or is the one being replaced by the “to” view controller.

## See Also

### Keys

static let to: UITransitionContextViewControllerKey

A key that identifies the view controller that’s visible at the end of a completed transition.

