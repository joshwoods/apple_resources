

- ARKit
- ARSCNPlaneGeometry
-  update(from:) 

Instance Method

# update(from:)

Reshapes the SceneKit geometry to match the specified plane mesh.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
func update(from planeGeometry: ARPlaneGeometry)
```

## Parameters 

`planeGeometry`  

A coarse mesh representation of a detected plane’s estimated shape.

## Discussion

To update a SceneKit model of a plane actively tracked in an AR session, call this method in your ARSCNViewDelegate object’s renderer(_:didUpdate:for:) callback, passing the geometry property from the ARPlaneAnchor object that callback provides.

