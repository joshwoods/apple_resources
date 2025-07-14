

- Create ML Components
- LinearRegressorModel
-  Regressor Implementations 

API Collection

# Regressor Implementations

## Topics

### Instance Methods

func prediction(from: Self.Input) async throws -> Self.Output

Performs a prediction from a single input.

func prediction&lt;S>(from: S) async throws -> [Self.Output]

Performs a prediction from a sequence of inputs.

