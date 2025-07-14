

- SceneKit
- SCNSceneSourceStatus
-  SCNSceneSourceStatus.validating 

Case

# SCNSceneSourceStatus.validating

SceneKit has begun validating the scene file’s format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case validating
```

## Discussion

If you specify true for the checkConsistency when creating or loading from a scene source, SceneKit verifies the scene file against the specification for its file format and reports any format consistency errors.

## See Also

### Constants

case error

An error occurred when SceneKit attempted to load the scene.

case parsing

SceneKit has begun deserializing the source file.

case processing

SceneKit has begun generating scene graph objects from the scene file’s contents.

case complete

SceneKit has successfully finished loading the scene file’s contents.

