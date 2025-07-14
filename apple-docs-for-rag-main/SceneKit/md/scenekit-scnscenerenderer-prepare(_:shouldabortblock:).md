

- SceneKit
- SCNSceneRenderer
-  prepare(\_:shouldAbortBlock:) 

Instance Method

# prepare(\_:shouldAbortBlock:)

Prepares a SceneKit object for rendering.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func prepare(
    _ object: Any,
    shouldAbortBlock block: (() -> Bool)? = nil
) -> Bool
```

**Required**

## Parameters 

`object`  

An SCNScene, SCNNode, SCNGeometry, or SCNMaterial instance.

`block`  

A block that SceneKit calls periodically while preparing the object. The block takes no parameters.

Your block should return false to tell SceneKit to continue preparing the object, or true to cancel preparation.

Pass `nil` for this parameter if you do not need an opportunity to cancel preparing the object.

## Return Value

true if the object was successfully prepared for rendering, or false if preparation was canceled.

## Discussion

By default, SceneKit lazily loads resources onto the GPU for rendering. This approach uses memory and GPU bandwidth efficiently, but can lead to stutters in an otherwise smooth frame rate when you add large amounts of new content to an animated scene. To avoid such issues, use this method to prepare content for drawing before adding it to the scene. You can call this method on a secondary thread to prepare content asynchronously.

SceneKit prepares all content associated with the `object` parameter you provide. If you provide an SCNMaterial object, SceneKit loads any texture images assigned to its material properties. If you provide an SCNGeometry object, SceneKit loads all materials attached to the geometry, as well as its vertex data. If you provide an SCNNode or SCNScene object, SceneKit loads all geometries and materials associated with the node and all its child nodes, or with the entire node hierarchy of the scene.

You can use the `block` parameter to cancel preparation if content is no longer needed. For example, in a game you might use this method to preload areas of the game world the player is soon to enter, but if the player character dies before entering those areas, you can return true from the block to cancel preloading.

You can observe the progress of this operation with the Progress class. For details, see Progress.

## See Also

### Preloading Renderer Resources

func prepare([Any], completionHandler: ((Bool) -> Void)?)

Prepares the specified SceneKit objects for rendering, using a background thread.

**Required**

