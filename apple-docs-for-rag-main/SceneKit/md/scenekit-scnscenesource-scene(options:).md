

- SceneKit
- SCNSceneSource
-  scene(options:) 

Instance Method

# scene(options:)

Instantiates a scene from the scene source with the specified options.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func scene(options: [SCNSceneSource.LoadingOption : Any]? = nil) throws -> SCNScene
```

## Parameters 

`options`  

A dictionary containing options that affect scene loading. See `Scene Loading Options` for available keys and values. Pass `nil` to use default options.

## Return Value

An SCNScene object containing the entire scene graph from the scene source, or `nil` if loading was not successful.

## Discussion

Calling this method is equivalent to calling scene(options:statusHandler:) with a block that checks its `error` parameter to see whether the status is SCNSceneSourceStatus.error. To load a scene without creating a scene source object, use the SCNScene method init(url:options:).

A scene source can contain objects that are not part of its scene graph. To obtain these objects, you must load them individually with the the entryWithIdentifier:withClass: or entries(passingTest:) method. For example, a scene file containing a game character could include several animations for the character geometry (such as running, jumping, and standing idle). Because you typically do not apply multiple animations at once, the scene file contains these animations without their being attached to the character geometry.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Loading a Complete Scene

func scene(options: [SCNSceneSource.LoadingOption : Any]?, statusHandler: SCNSceneSourceStatusHandler?) -> SCNScene?

Loads the entire scene graph from the scene source and calls the specified block to provide progress information.

