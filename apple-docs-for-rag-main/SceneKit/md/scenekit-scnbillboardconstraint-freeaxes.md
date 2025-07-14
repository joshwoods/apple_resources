

- SceneKit
- SCNBillboardConstraint
-  freeAxes 

Instance Property

# freeAxes

An option that specifies which degrees of freedom the constraint affects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var freeAxes: SCNBillboardAxis { get set }
```

## Discussion

With the default constraint type of all, a node affected by the constraint never rotates with respect to the scene’s point of view. Change this property to partially constrain a node’s orientation. For example, the Y constraint type keeps only the node’s y-axis parallel to the screen—this option can be useful for applications like drawing trees in the distance with 2D sprites instead of with 3D geometry.

