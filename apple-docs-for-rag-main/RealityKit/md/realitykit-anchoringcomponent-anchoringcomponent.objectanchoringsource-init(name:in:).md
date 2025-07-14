

- RealityKit
- AnchoringComponent
- AnchoringComponent.ObjectAnchoringSource
-  init(name:in:) 

Initializer

# init(name:in:)

Creates the object anchoring source by reference object file asset with provided name and bundle.

Mac Catalyst 18.0+visionOS 2.0+

``` source
init(
    name: String,
    in bundle: Bundle = .main
)
```

## Parameters 

`name`  

The name of the reference object in the bundle.

`bundle`  

The bundle to load from.

