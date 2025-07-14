

- SwiftUI
- View
-  modelContext(\_:) 

Instance Method

# modelContext(\_:)

Sets the model context in this view’s environment.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func modelContext(_ modelContext: ModelContext) -> some View
```

## Parameters 

`modelContext`  

The model context to set in this view’s environment.

## Discussion

In this example, the `RecipesList` view sets a model context to use for all of its content:

```
@Model class Recipe { ... }
...
RecipesList()
    .modelContext(myContext)
```

The environment’s modelContext property will be assigned `myContext`. All implicit model context operations in this view, such as `Query` properties, will use the environment’s context.

## See Also

### Configuring a model

func modelContainer(ModelContainer) -> some View

Sets the model container and associated model context in this view’s environment.

func modelContainer(for:inMemory:isAutosaveEnabled:isUndoEnabled:onSetup:)

Sets the model container in this view for storing the provided model type, creating a new container if necessary, and also sets a model context for that container in this view’s environment.

