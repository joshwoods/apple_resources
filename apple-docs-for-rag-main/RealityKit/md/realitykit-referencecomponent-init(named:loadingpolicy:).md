

- RealityKit
- ReferenceComponent
-  init(named:loadingPolicy:) 

Initializer

# init(named:loadingPolicy:)

Creates a reference component with a name and loading policy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    named name: String,
    loadingPolicy: ReferenceComponent.LoadingPolicy = .onDemand
)
```

## Parameters 

`name`  

The name of the entity to load.

`loadingPolicy`  

A loading policy indicating when the app loads the entity.

## Discussion

Place references in the app’s main bundle.

