

- SceneKit
- SCNNode
-  constraints 

Instance Property

# constraints

A list of constraints affecting the node’s transformation.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var constraints: [SCNConstraint]? { get set }
```

## Discussion

An array of constraint objects. Before rendering, SceneKit evaluates all constraints attached to a node hierarchy and adjusts node transformations appropriately.

Use the SCNLookAtConstraint class to make a node always point toward another node even as both are moved, or the SCNTransformConstraint class to apply arbitrary transformations at constraint evaluation time.

