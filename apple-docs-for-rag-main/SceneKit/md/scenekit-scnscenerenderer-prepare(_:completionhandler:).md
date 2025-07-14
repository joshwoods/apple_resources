

- SceneKit
- SCNSceneRenderer
-  prepare(\_:completionHandler:) 

Instance Method

# prepare(\_:completionHandler:)

Prepares the specified SceneKit objects for rendering, using a background thread.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func prepare(
    _ objects: [Any],
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func prepare(_ objects: [Any]) async -> Bool
```

**Required**

## Parameters 

`objects`  

An array of containing one or more SCNScene, SCNNode, SCNGeometry, or SCNMaterial instances.

`completionHandler`  

A block that SceneKit calls when object preparation fails or completes.

The block takes the following parameter:

success  
true if all content was successfully prepared for rendering; otherwise, false.

## Discussion

Concurrency Note

In Swift, you can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func prepare(_ objects: [Any]) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

By default, SceneKit lazily loads resources onto the GPU for rendering. This approach uses memory and GPU bandwidth efficiently, but can lead to stutters in an otherwise smooth frame rate when you add large amounts of new content to an animated scene. To avoid such issues, use this method to prepare content for drawing before adding it to the scene. SceneKit uses a secondary thread to prepare content asynchronously.

SceneKit prepares all content associated with the objects you provide. If you provide an SCNMaterial object, SceneKit loads any texture images assigned to its material properties. If you provide an SCNGeometry object, SceneKit loads all materials attached to the geometry, as well as its vertex data. If you provide an SCNNode or SCNScene object, SceneKit loads all geometries and materials associated with the node and all its child nodes, or with the entire node hierarchy of the scene.

You can observe the progress of this operation with the Progress class. For details, see Progress.

## See Also

### Preloading Renderer Resources

func prepare(Any, shouldAbortBlock: (() -> Bool)?) -> Bool

Prepares a SceneKit object for rendering.

**Required**

