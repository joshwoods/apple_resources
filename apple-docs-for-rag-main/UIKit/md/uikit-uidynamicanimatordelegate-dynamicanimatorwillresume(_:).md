

- UIKit
- UIDynamicAnimatorDelegate
-  dynamicAnimatorWillResume(\_:) 

Instance Method

# dynamicAnimatorWillResume(\_:)

Called when a dynamic animator is about to resume the animations for its behaviors’ associated dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func dynamicAnimatorWillResume(_ animator: UIDynamicAnimator)
```

## Parameters 

`animator`  

The dynamic animator that is about to resume animation.

## See Also

### Responding to animation pausing and resumption

func dynamicAnimatorDidPause(UIDynamicAnimator)

Called when a dynamic animator pauses the animations for its behaviors’ associated dynamic items.

