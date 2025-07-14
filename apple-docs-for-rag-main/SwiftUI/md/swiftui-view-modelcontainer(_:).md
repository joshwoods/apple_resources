

- SwiftUI
- View
-  modelContainer(\_:) 

Instance Method

# modelContainer(\_:)

Sets the model container and associated model context in this view’s environment.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func modelContainer(_ container: ModelContainer) -> some View
```

## Parameters 

`container`  

The model container to use for this view.

## Discussion

In this example, `ContentView` sets a model container to use for `RecipesList`:

```
struct ContentView: View {
    @State private var container = ModelContainer(...)

    var body: some Scene {
        RecipesList()
            .modelContainer(container)
    }
}
```

The environment’s modelContext property will be assigned a new context associated with this container. All implicit model context operations in this view, such as `Query` properties, will use the environment’s context.

## See Also

### Configuring a model

func modelContext(ModelContext) -> some View

Sets the model context in this view’s environment.

func modelContainer(for:inMemory:isAutosaveEnabled:isUndoEnabled:onSetup:)

Sets the model container in this view for storing the provided model type, creating a new container if necessary, and also sets a model context for that container in this view’s environment.

