

- Core ML
-  MLState 

Class

# MLState

Handle to the state buffers.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class MLState
```

## Overview

A stateful model maintains a state from one prediction to another by storing the information in the state buffers. To use such a model, the client must request the model to create state buffers and get `MLState` object, which is the handle to those buffers. Then, at the prediction time, pass the `MLState` object in one of the stateful prediction functions.

```
// Load a stateful model
let modelAsset = try MLModelAsset(url: modelURL)
let model = try await MLModel.load(asset: modelAsset, configuration: MLModelConfiguration())

// Request a state
let state = model.newState()

// Run predictions
for _ in 0 ..

The object is a handle to the state buffers. The client shall not read or write the buffers while a prediction is in-flight.

Each stateful prediction that uses the same `MLState` must be serialized. Otherwise, if two such predictions run concurrently, the behavior is undefined.

## Topics

### Instance Methods

func withMultiArray&lt;R>((MLMultiArray) -> R) throws -> RDeprecated

func withMultiArray&lt;R>(for: String, (MLMultiArray) throws -> R) rethrows -> R

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Model state

class MLStateConstraint

Constraint of a state feature value.

