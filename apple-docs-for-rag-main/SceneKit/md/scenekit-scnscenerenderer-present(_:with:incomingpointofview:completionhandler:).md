

- SceneKit
- SCNSceneRenderer
-  present(\_:with:incomingPointOfView:completionHandler:) 

Instance Method

# present(\_:with:incomingPointOfView:completionHandler:)

Displays the specified scene with an animated transition.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func present(
    _ scene: SCNScene,
    with transition: SKTransition,
    incomingPointOfView pointOfView: SCNNode?,
    completionHandler: (() -> Void)? = nil
)
```

``` source
func present(
    _ scene: SCNScene,
    with transition: SKTransition,
    incomingPointOfView pointOfView: SCNNode?
) async
```

**Required**

## Parameters 

`scene`  

The new scene to be displayed.

`transition`  

An object that specifies the duration and style of the animated transition.

`pointOfView`  

The node to use as the pointOfView property when displaying the new scene.

`completionHandler`  

A block that SceneKit calls after the transition animation has completed.

This block takes no parameters and has no return value.

## Discussion

Concurrency Note

In Swift, you can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func present(_ scene: SCNScene, with transition: SKTransition, incomingPointOfView pointOfView: SCNNode?) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to change the scene displayed in a SceneKit view (or other renderer) with an animated transition. For details on transition styles, see SKTransition.

## See Also

### Presenting a Scene

var scene: SCNScene?

The scene to be displayed.

**Required**

