

- RealityKit
- Entity
-  loadAnchor(contentsOf:withName:) 

Type Method

# loadAnchor(contentsOf:withName:)

Synchronously loads an anchor entity from a file URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func loadAnchor(
    contentsOf url: URL,
    withName resourceName: String? = nil
) throws -> AnchorEntity
```

## Parameters 

`url`  

A file URL representing the file to load.

`resourceName`  

A unique name the method assigns to the resource it loads, for use in network synchronization.

## Return Value

The root entity in the loaded file, which Reality Kit casts as an AnchorEntity.

## Mentioned in 

Taking Control of Scene Anchoring

Loading Reality Composer files manually without generated code

## Discussion

Loading an Entity with this method blocks the main actor because it’s synchronous, so only call it from a command-line application. The method can stall a regular app, which makes it visibly hitch, and the system terminates an app if its UI becomes unresponsive. See init(named:in:) for an example that demonstrates how to safely load content.

## See Also

### Loading an anchor entity

static func loadAnchor(named: String, in: Bundle?) throws -> AnchorEntity

Synchronously loads an anchor entity from a bundle.

static func loadAnchorAsync(named: String, in: Bundle?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a bundle.

Deprecated

static func loadAnchorAsync(contentsOf: URL, withName: String?) -> LoadRequest&lt;AnchorEntity>

Asynchronously loads an anchor entity from a file URL.

Deprecated

