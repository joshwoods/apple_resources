

- SpriteKit
- SKCameraNode
-  containedNodeSet() 

Instance Method

# containedNodeSet()

Finds nodes that are visible in the camera’s viewport.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
func containedNodeSet() -> Set
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func containedNodeSet() -> Set
```

## Return Value

The set of nodes that are in the same scene as the camera and contained in the camera’s viewport.

## Discussion

The camera must be part of a scene’s node hierarchy and the scene must be presented in an view.

## See Also

### Node Visibility

func contains(SKNode) -> Bool

Checks to see if a node is visible in the camera’s viewport.

