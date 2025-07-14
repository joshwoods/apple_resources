

- RealityKit
- Entity
-  loadBodyTracked(contentsOf:withName:) 

Type Method

# loadBodyTracked(contentsOf:withName:)

Synchronously loads a body-tracked entity from a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
static func loadBodyTracked(
    contentsOf url: URL,
    withName resourceName: String? = nil
) throws -> BodyTrackedEntity
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

The root entity in the loaded file, cast as a BodyTrackedEntity.

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading a flattened body-tracked entity

static func loadBodyTracked(named: String, in: Bundle?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a bundle.

static func loadBodyTrackedAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(named: String, in: Bundle?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a bundle.

Deprecated

