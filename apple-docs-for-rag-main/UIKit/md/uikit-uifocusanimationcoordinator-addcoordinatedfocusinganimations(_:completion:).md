

- UIKit
- UIFocusAnimationCoordinator
-  addCoordinatedFocusingAnimations(\_:completion:) 

Instance Method

# addCoordinatedFocusingAnimations(\_:completion:)

Runs the specified set of animations together with the system animations for adding focus to an item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func addCoordinatedFocusingAnimations(
    _ animations: ((any UIFocusAnimationContext) -> Void)?,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`animations`  

A block object containing your focus-related animations. This block has no return value and takes the following parameter:

context  
An object containing information about the main animations. Use this information to configure your custom animations. For more information, see UIFocusAnimationContext.

`completion`  

The block object to execute after the main animations completes. The specified animations are run in the same animation context as the main animation.

## Discussion

When focus is being added to an item, use this method to coordinate your custom animations with the system animations. The animations you specify are run in the same animation block as the system animations. Use the information in the context parameter to determine any custom behaviors for your animations. For example, you might configure your animations to run in half the time as the main animation and start after a short delay.

## See Also

### Adding animations to focus updates

func addCoordinatedUnfocusingAnimations(((any UIFocusAnimationContext) -> Void)?, completion: (() -> Void)?)

Runs the specified set of animations together with the system animations for removing focus from an item.

func addCoordinatedAnimations((() -> Void)?, completion: (() -> Void)?)

Specifies the animations to coordinate with the active focus animation.

protocol UIFocusAnimationContext

Information about focusing animations being performed by the system.

