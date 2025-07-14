

- AVKit
- AVPlayerViewControllerAnimationCoordinator
-  addCoordinatedAnimations(\_:completion:) 

Instance Method

# addCoordinatedAnimations(\_:completion:)

Adds animations to perform alongside the playback controls’ visibility animation.

tvOS 11.0+

``` source
func addCoordinatedAnimations(
    _ animations: (() -> Void)?,
    completion: ((Bool) -> Void)? = nil
)
```

``` source
func addCoordinatedAnimations(_ animations: (() -> Void)?) async -> Bool
```

**Required**

## Parameters 

`animations`  

The animations to execute.

`completion`  

A closure to execute after the main animation completes. The system runs the specified animations in the same animation context as the main animation.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func addCoordinatedAnimations(_ animations: (() -> Void)?) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

