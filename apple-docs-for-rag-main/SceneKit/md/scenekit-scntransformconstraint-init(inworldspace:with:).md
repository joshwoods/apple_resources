

- SceneKit
- SCNTransformConstraint
-  init(inWorldSpace:with:) 

Initializer

# init(inWorldSpace:with:)

Creates a new transform constraint.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

**macOS**

``` source
convenience init(
    inWorldSpace world: Bool,
    with block: @escaping (SCNNode, SCNMatrix4) -> SCNMatrix4
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
convenience init(
    inWorldSpace world: Bool,
    with block: @escaping (SCNNode, SCNMatrix4) -> SCNMatrix4
)
```

## Parameters 

`world`  

true to evaluate the constraint in the scene’s world coordinate space, or false to evaluate it relative to the local coordinate space of each constrained node.

`block`  

A block to be called when Scene Kit evaluates the constraint.

The block takes the following parameters:

node  
The constrained node.

transform  
The constrained node’s current presentation transformation—the value of the transform property of the constrained node’s presentation object. If the node is affected by an in-progress animation, this value reflects the currently visible state of the node during the animation (rather than its target state that will be visible when the animation completes).

The block returns a transformation matrix, which Scene Kit then applies to the node. If you return the `transform` value passed to the block, your constraint has no effect on the node.

## Return Value

A constraint object.

## Discussion

The `world` parameter determines the coordinate space of the transformations passed to and returned by the `block` parameter.

