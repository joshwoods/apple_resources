

- App Intents
-  IntentPredictionsBuilder 

Enumeration

# IntentPredictionsBuilder

A result builder that allows you to declaratively describe the predictions for an app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum IntentPredictionsBuilder where Intent : AppIntent
```

## Topics

### Building predictions

static func buildBlock&lt;A0>(A0) -> A0

static func buildBlock&lt;A0, A1>(A0, A1) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1)>

static func buildBlock&lt;A0, A1, A2>(A0, A1, A2) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2)>

struct TupleIntentPrediction

A type that represents a collection of predictions for a specific app intent.

### Type Methods

static func buildBlock&lt;A0, A1, A2, A3>(A0, A1, A2, A3) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3)>

static func buildBlock&lt;A0, A1, A2, A3, A4>(A0, A1, A2, A3, A4) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5>(A0, A1, A2, A3, A4, A5) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6>(A0, A1, A2, A3, A4, A5, A6) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7>(A0, A1, A2, A3, A4, A5, A6, A7) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8>(A0, A1, A2, A3, A4, A5, A6, A7, A8) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13)>

static func buildBlock&lt;A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13, A14>(A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13, A14) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2, A3, A4, A5, A6, A7, A8, A9, A10, A11, A12, A13, A14)>

static func buildExpression&lt;A0>(A0) -> A0

## See Also

### Providing predictions

static var predictionConfiguration: Self.Prediction

A collection of predictions the system can use when it suggests the app intent.

**Required**

protocol IntentPredictionConfiguration

An interface that provides the configuration for a single prediction.

