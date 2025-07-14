

- SceneKit
- SCNSceneSourceStatus
-  SCNSceneSourceStatus.error 

Case

# SCNSceneSourceStatus.error

An error occurred when SceneKit attempted to load the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case error
```

## Discussion

If the `status` parameter of a SCNSceneSourceStatusHandler block has this value, see the block’s `error` parameter for information about the nature and location of the error. When SceneKit encounters an error during scene loading, it calls the handler block with this status, then after the block completes, the scene(options:statusHandler:) method returns `nil`.

## See Also

### Constants

case parsing

SceneKit has begun deserializing the source file.

case validating

SceneKit has begun validating the scene file’s format.

case processing

SceneKit has begun generating scene graph objects from the scene file’s contents.

case complete

SceneKit has successfully finished loading the scene file’s contents.

