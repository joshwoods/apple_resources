

- SwiftData
-  ModelActor 

Protocol

# ModelActor

An interface for providing mutually-exclusive access to the attributes of a conforming model.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol ModelActor : Actor
```

## Topics

### Accessing the container and context

var modelContainer: ModelContainer

The ModelContainer for the ModelActor The container that manages the app’s schema and model storage configuration

**Required**

var modelContext: ModelContext

The context that serializes any code running on the model actor.

### Accessing the executors

var modelExecutor: any ModelExecutor

The executor that coordinates access to the model actor.

**Required**

var unownedExecutor: UnownedSerialExecutor

The optimized, unonwned reference to the model actor’s executor.

### Accessing specific models

subscript&lt;T>(PersistentIdentifier, as _: T.Type) -> T?

Returns the model for the specified identifier, downcast to the appropriate class.

## Relationships

### Inherits From

- Actor
- Sendable

## See Also

### Model actors

macro ModelActor()

Converts a Swift actor into a model actor by generating boilerplate code that fulfills the requirements of the associated protocol.

