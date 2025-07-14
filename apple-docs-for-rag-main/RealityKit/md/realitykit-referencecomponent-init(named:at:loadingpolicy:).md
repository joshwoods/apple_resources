

- RealityKit
- ReferenceComponent
-  init(named:at:loadingPolicy:) 

Initializer

# init(named:at:loadingPolicy:)

Creates a reference component with a name, loading policy, and bundle path.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    named name: String,
    at bundlePath: String = "",
    loadingPolicy: ReferenceComponent.LoadingPolicy = .onDemand
)
```

## Parameters 

`name`  

The name of the entity to load.

`bundlePath`  

The bundle path to search for the resource. Specify the path relative to the Resources directory.

`loadingPolicy`  

A loading policy that indicates when the app loads the entity.

