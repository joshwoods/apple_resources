

- GLKit
- GLKViewControllerDelegate
-  glkViewControllerUpdate(\_:) 

Instance Method

# glkViewControllerUpdate(\_:)

Called before each frame is displayed.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
func glkViewControllerUpdate(_ controller: GLKViewController)
```

**Required**

## Parameters 

`controller`  

The controller that is about to display a new frame.

## Discussion

This method is used by your application if it wants to updates state information on each frame of animation. A typical implementation might read the controller’s timeSinceLastUpdate property to determine how much time has actually passed, and use that time to calculate the positions for any objects to be rendered in the next frame.

