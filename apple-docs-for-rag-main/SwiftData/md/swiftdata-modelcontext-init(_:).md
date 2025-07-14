

- SwiftData
- ModelContext
-  init(\_:) 

Initializer

# init(\_:)

Creates a context that belongs to the specified model container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
init(_ container: ModelContainer)
```

## Parameters 

`container`  

The model container to associate with the initialized context.

## Discussion

Use the context’s container property to access the model container after initializtion.

## See Also

### Creating a model context

class ModelContainer

An object that manages an app’s schema and model storage configuration.

