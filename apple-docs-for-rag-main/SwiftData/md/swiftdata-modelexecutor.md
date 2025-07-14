

- SwiftData
-  ModelExecutor 

Protocol

# ModelExecutor

An interface for performing storage-related tasks using an isolated model context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
protocol ModelExecutor : Executor
```

## Topics

### Accessing the context

var modelContext: ModelContext

**Required**

## Relationships

### Inherits From

- Executor
- Sendable

### Inherited By

- SerialModelExecutor

### Conforming Types

- DefaultSerialModelExecutor

## See Also

### Model executors

class DefaultSerialModelExecutor

An object that safely performs storage-related tasks using an isolated model context.

protocol SerialModelExecutor

An interface for performing serial storage-related tasks using an isolated model context.

