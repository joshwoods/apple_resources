

- App Intents
- IntentPredictionsBuilder
-  buildBlock(\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildBlock(
    _ a0: A0,
    _ a1: A1,
    _ a2: A2
) -> TupleIntentPrediction where Intent == A0.Intent, A0 : IntentPredictionConfiguration, A1 : IntentPredictionConfiguration, A2 : IntentPredictionConfiguration, A0.Intent == A1.Intent, A1.Intent == A2.Intent
```

Available when `Intent` conforms to `AppIntent`.

## See Also

### Building predictions

static func buildBlock&lt;A0>(A0) -> A0

static func buildBlock&lt;A0, A1>(A0, A1) -> TupleIntentPrediction&lt;A0.Intent, (A0, A1)>

struct TupleIntentPrediction

A type that represents a collection of predictions for a specific app intent.

