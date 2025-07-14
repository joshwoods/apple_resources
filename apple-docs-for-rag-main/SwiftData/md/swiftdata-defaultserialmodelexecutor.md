

- SwiftData
-  DefaultSerialModelExecutor 

Class

# DefaultSerialModelExecutor

An object that safely performs storage-related tasks using an isolated model context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
class DefaultSerialModelExecutor
```

## Topics

### Creating a model executor

init(modelContext: ModelContext)

### Accessing the context

let modelContext: ModelContext

### Default Implementations

SerialExecutor Implementations

## Relationships

### Conforms To

- Copyable
- Executor
- ModelExecutor
- Sendable
- SerialExecutor
- SerialModelExecutor

## See Also

### Model executors

protocol SerialModelExecutor

An interface for performing serial storage-related tasks using an isolated model context.

protocol ModelExecutor

An interface for performing storage-related tasks using an isolated model context.

