

- RealityKit
- Entity
-  loadBodyTrackedAsync(contentsOf:withName:) 

Type Method

# loadBodyTrackedAsync(contentsOf:withName:)

Asynchronously loads a body-tracked entity from a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
static func loadBodyTrackedAsync(
    contentsOf url: URL,
    withName resourceName: String? = nil
) -> LoadRequest
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

A resource loader that publishes the root entity in the loaded file as a BodyTrackedEntity.

## See Also

### Loading a flattened body-tracked entity

static func loadBodyTracked(named: String, in: Bundle?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a bundle.

static func loadBodyTracked(contentsOf: URL, withName: String?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(named: String, in: Bundle?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a bundle.

Deprecated

