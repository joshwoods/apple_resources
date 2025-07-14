

- RealityKit
- Entity
-  loadBodyTracked(named:in:) 

Type Method

# loadBodyTracked(named:in:)

Synchronously loads a body-tracked entity from a bundle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
static func loadBodyTracked(
    named name: String,
    in bundle: Bundle? = nil
) throws -> BodyTrackedEntity
```

## Parameters 

`name`  

The base name of the file to load, omitting the filename extension.

`bundle`  

The bundle containing the file. Use `nil` to search the app’s main bundle.

## Return Value

The root entity in the loaded file, cast as a BodyTrackedEntity.

## Mentioned in 

Loading entities from a file

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading a flattened body-tracked entity

static func loadBodyTracked(contentsOf: URL, withName: String?) throws -> BodyTrackedEntity

Synchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a file URL.

static func loadBodyTrackedAsync(named: String, in: Bundle?) -> LoadRequest&lt;BodyTrackedEntity>

Asynchronously loads a body-tracked entity from a bundle.

Deprecated

