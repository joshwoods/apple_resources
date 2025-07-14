

- SceneKit
- SCNLookAtConstraint
-  init(target:) 

Initializer

# init(target:)

Creates a look-at constraint for a specified target node.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init(target: SCNNode?)
```

## Parameters 

`target`  

The node that constrained nodes will be reoriented to point toward.

## Return Value

A constraint object.

## Discussion

To attach constraints to an SCNNode object, use its constraints property.

