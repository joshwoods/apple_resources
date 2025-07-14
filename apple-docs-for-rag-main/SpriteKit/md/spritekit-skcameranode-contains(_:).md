

- SpriteKit
- SKCameraNode
-  contains(\_:) 

Instance Method

# contains(\_:)

Checks to see if a node is visible in the camera’s viewport.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
func contains(_ node: SKNode) -> Bool
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func contains(_ node: SKNode) -> Bool
```

## Parameters 

`node`  

An SKNode object.

## Return Value

true if the node in the same scene and inside the camera’s viewport; otherwise false.

## Discussion

The camera must be part of a scene’s node hierarchy and the scene must be presented in an view.

## See Also

### Node Visibility

func containedNodeSet() -> Set&lt;SKNode>

Finds nodes that are visible in the camera’s viewport.

