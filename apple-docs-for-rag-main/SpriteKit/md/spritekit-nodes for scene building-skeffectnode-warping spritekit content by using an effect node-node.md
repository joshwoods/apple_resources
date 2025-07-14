

- SpriteKit
- Nodes for Scene Building
- SKEffectNode
-  Warping SpriteKit Content By Using an Effect Node 

Article

# Warping SpriteKit Content By Using an Effect Node

Distort the child nodes of an effect node by applying a warping effect.

## Overview

If you want to warp a node that doesn’t conform to SKWarpable, you can add it as a child to an effect node that is warped. As an implementor of `SKWarpable`, effect node inherits the SKWarpGeometry property that you assign one of the SKWarpGeometry types to then warp the effect node’s children.

### Warp Text By Using an Effect Node

SKLabelNode is one such class that doesn’t conform to `SKWarpable`. The following Swift code shows how you can warp a label node by adding it as a child to a SKEffectNode and assign the effect node a SKWarpGeometryGrid that pulls out the corners horizontally and stretches the center vertically.

```
let labelNode = SKLabelNode(text: "SpriteKit")
labelNode.fontColor = UIColor.blue
labelNode.fontSize = 144

let effectNode = SKEffectNode()
effectNode.addChild(labelNode)

let destinationPositions: [vector_float2] = [
    vector_float2(-0.1, 1), vector_float2(0.5, 1.3), vector_float2(1.1, 1),
    vector_float2(0.1, 0.5), vector_float2(0.5, 0.5), vector_float2(0.9, 0.5),
    vector_float2(-0.1, 0), vector_float2(0.5, -0.3), vector_float2(1.1, 0)
]

let warpGeometryGrid = SKWarpGeometryGrid(columns: 2,
                                          rows: 2)

effectNode.warpGeometry = warpGeometryGrid.replacingByDestinationPositions(positions: destinationPositions)
```

The following image shows the warped label.

