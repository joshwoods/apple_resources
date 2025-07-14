

- App Intents
- IntentPredictionsBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildBlock(_ block: A0) -> A0 where Intent == A0.Intent, A0 : IntentPredictionConfiguration
```

## See Also

### Building predictions

static func buildBlock&lt;A0, A1>(A0, A1) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1)>

static func buildBlock&lt;A0, A1, A2>(A0, A1, A2) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1, A2)>

struct TupleIntentPrediction

A type that represents a collection of predictions for a specific app intent.

