

- SceneKit
- SCNSceneSource
-  scene(options:statusHandler:) 

Instance Method

# scene(options:statusHandler:)

Loads the entire scene graph from the scene source and calls the specified block to provide progress information.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func scene(
    options: [SCNSceneSource.LoadingOption : Any]? = nil,
    statusHandler: SCNSceneSourceStatusHandler? = nil
) -> SCNScene?
```

## Parameters 

`options`  

A dictionary containing options that affect scene loading. See `Scene Loading Options` for available keys and values. Pass `nil` to use default options.

`statusHandler`  

An SCNSceneSourceStatusHandler block. SceneKit calls this block periodically to report progress while loading the scene.

## Return Value

An SCNScene object containing the entire scene graph from the scene source, or `nil` if loading was not successful.

## Discussion

Use this method if you need to monitor progress while loading a scene from the scene source. For simpler scene loading, use the scene(options:) method or the SCNScene method init(url:options:).

A scene source can contain objects that are not part of its scene graph. To obtain these objects, you must load them individually with the the entryWithIdentifier:withClass: or entries(passingTest:) method. For example, a scene file containing a game character could include several animations for the character geometry (such as running, jumping, and standing idle). Because you typically do not apply multiple animations at once, the scene file contains these animations without their being attached to the character geometry.

## See Also

### Loading a Complete Scene

func scene(options: [SCNSceneSource.LoadingOption : Any]?) throws -> SCNScene

Instantiates a scene from the scene source with the specified options.

