

- RealityKit
- IKResource
-  init(rig:) 

Initializer

# init(rig:)

Creates a new resource instance for a single solver using the given rig and an automatic solver identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
convenience init(rig: IKRig) throws
```

## Parameters 

`rig`  

The inverse kinematics rig to be serialised into the resource.

## Discussion

Throws

Validation errors for the given rig structure.

