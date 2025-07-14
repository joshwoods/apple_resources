

- ARKit
- ARSCNPlaneGeometry
-  init(device:) 

Initializer

# init(device:)

Creates a SceneKit plane geometry for rendering with the specified Metal device object.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
convenience init?(device: any MTLDevice)
```

## Parameters 

`device`  

The Metal device to use for rendering the geometry.

## Return Value

A new SceneKit plane geometry, or `nil` if the Metal device is unavailable.

## Discussion

A newly created ARSCNPlaneGeometry instance does not represent any specific plane; use the update(from:) method to make the geometry match the estimated shape of a specific plane anchor.

The geometry contains a single geometry element; as such, assigning more than one material has no visible effect (see the inherited materials property).

