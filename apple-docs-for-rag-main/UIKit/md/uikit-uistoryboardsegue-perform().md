

- UIKit
- UIStoryboardSegue
-  perform() 

Instance Method

# perform()

Performs the visual transition for the segue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func perform()
```

## Discussion

Subclasses override this method and use it to perform the animations from the views in source to the views in destination. Typically, you use UIKit or Core Animation to set up an animation from one set of views to the next. For more complex animations, you might take a snapshot image of the two view hierarchies and manipulate the images instead of the actual view objects.

Regardless of how you perform the animation, at the end of it, you’re responsible for installing the destination view controller (and its views) in the right place so that it can handle events. For example, if you were to implement a custom modal transition, you might perform your animations using snapshot images and then at the end call the presentModalViewController:animated: method (with animations disabled) to set up the appropriate modal relationship between the source and destination view controllers.

