

- RealityKit
- ReferenceComponent
-  init(named:in:loadingPolicy:) 

Initializer

# init(named:in:loadingPolicy:)

Creates a reference component with a name, loading policy, and bundle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    named name: String,
    in bundle: Bundle,
    loadingPolicy: ReferenceComponent.LoadingPolicy = .onDemand
)
```

## Parameters 

`name`  

The name of the entity to load.

`bundle`  

The bundle to search for the resource.

`loadingPolicy`  

A loading policy indicating when the app loads the entity.

