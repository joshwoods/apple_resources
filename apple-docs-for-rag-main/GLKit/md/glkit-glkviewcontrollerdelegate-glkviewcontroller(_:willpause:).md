

- GLKit
- GLKViewControllerDelegate
-  glkViewController(\_:willPause:) 

Instance Method

# glkViewController(\_:willPause:)

Called before the rendering loop is paused or resumed.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
optional func glkViewController(
    _ controller: GLKViewController,
    willPause pause: Bool
)
```

## Parameters 

`controller`  

The controller that is about to change the rendering loop state.

`pause`  

true if the loop is being paused, false if it is being resumed.

