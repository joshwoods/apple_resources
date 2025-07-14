

- RealityKit
- Entity
-  loadAnchor(named:in:) 

Type Method

# loadAnchor(named:in:)

Synchronously loads an anchor entity from a bundle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func loadAnchor(
    named name: String,
    in bundle: Bundle? = nil
) throws -> AnchorEntity
```

## Parameters 

`name`  

The base name of the file to load, omitting the filename extension.

`bundle`  

The bundle containing the file. Use `nil` to search the app’s main bundle.

## Return Value

The root entity in the loaded file, which Reality Kit casts as an AnchorEntity.

## Mentioned in 

Loading entities from a file

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading an anchor entity

static func loadAnchor(contentsOf: URL, withName: String?) throws -> AnchorEntity

Synchronously loads an anchor entity from a file URL.

static func loadAnchorAsync(named: String, in: Bundle?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a bundle.

Deprecated

static func loadAnchorAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a file URL.

Deprecated

