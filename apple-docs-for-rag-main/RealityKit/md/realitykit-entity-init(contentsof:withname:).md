

- RealityKit
- Entity
-  init(contentsOf:withName:) 

Initializer

# init(contentsOf:withName:)

Creates an entity by asynchronously loading it from a file URL.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    contentsOf url: URL,
    withName resourceName: String? = nil
) async throws
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

The root entity of the loaded file.

## Discussion

RealityKit supports loading entities from USD (`.usd`, `.usda`, `.usdc`, `.usdz`) and Reality (`.reality`) files.

For more information on loading entities, see Loading entities from a file.

See init(named:in:) for an example of optimally loading content.

## See Also

### Loading an entity from a file

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

Stored entities

Manage entities that you store as assets on disk.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

convenience init(named: String, in: Bundle?) async throws

Creates an entity by asynchronously loading it from a bundle.

struct ReferenceComponent

A component that can load another entity from a file.

