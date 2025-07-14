

- SwiftUI
- Scene
-  modelContainer(\_:) 

Instance Method

# modelContainer(\_:)

Sets the model container and associated model context in this scene’s environment.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func modelContainer(_ container: ModelContainer) -> some Scene
```

## Parameters 

`container`  

The model container to use for this scene.

## Discussion

In this example, `RecipesApp` sets a shared model container to use for all of its windows:

```
@main
struct RecipesApp: App {
    @State private var container = ModelContainer(...)

    var body: some Scene {
        WindowGroup {
            RecipesList()
        }
        .modelContainer(container)
    }
}
```

The environment’s modelContext property will be assigned a new context associated with this container. All implicit model context operations in this scene, such as `Query` properties, will use the environment’s context.

## See Also

### Configuring a data model

func modelContext(ModelContext) -> some Scene

Sets the model context in this scene’s environment.

func modelContainer(for:inMemory:isAutosaveEnabled:isUndoEnabled:onSetup:)

Sets the model container in this scene for storing the provided model type, creating a new container if necessary, and also sets a model context for that container in this scene’s environment.

