

- RealityKit
- Entity
-  init(named:in:) 

Initializer

# init(named:in:)

Creates an entity by asynchronously loading it from a bundle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(
    named name: String,
    in bundle: Bundle? = nil
) async throws
```

## Parameters 

`name`  

The base name of the file to load, omitting the filename extension, or scene name if loading from a `.reality` file.

`bundle`  

The bundle containing the file. Use `nil` to search the app’s main bundle.

## Return Value

The root entity in the loaded file.

## Discussion

RealityKit supports loading entities from USD (`.usd`, `.usda`, `.usdc`, `.usdz`) and Reality (`.reality`) files.

For more information on loading entities, see Loading entities from a file.

You can use a task group to await all loads before adding them to the scene to display content from multiple scenes without hitches or pop-in.

```
struct SomeRealityView: View {
    var body: some View {
        RealityView { content in
            // Add the initial RealityKit content.
            let entities : [Entity] = await withTaskGroup(of: Entity?.self) { taskGroup in
                // Load all the scenes concurrently.
                taskGroup.addTask { return try? await Entity(named: "SceneA", in: realityKitContentBundle) }
                taskGroup.addTask { return try? await Entity(named: "SceneB", in: realityKitContentBundle) }
                taskGroup.addTask { return try? await Entity(named: "SceneC", in: realityKitContentBundle) }

                var entities = [Entity]()
                // Wait for all the scenes to load.
                for await entity in taskGroup {
                    if let entity {
                        entities.append(entity)
                    }
                }
                return entities
            }
            // Add all the content.
            for entity in entities {
                content.add(entity)
            }
        }
    }
}
```

## See Also

### Loading an entity from a file

Loading entities from a file

Retrieve an entity from storage on disk using a synchronous or an asynchronous load operation.

Stored entities

Manage entities that you store as assets on disk.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

convenience init(contentsOf: URL, withName: String?) async throws

Creates an entity by asynchronously loading it from a file URL.

struct ReferenceComponent

A component that can load another entity from a file.

