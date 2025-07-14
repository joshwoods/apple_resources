

- App Intents
- PredictableIntent
-  predictionConfiguration 

Type Property

# predictionConfiguration

A collection of predictions the system can use when it suggests the app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@IntentPredictionsBuilder static var predictionConfiguration: Self.Prediction { get }
```

**Required**

## See Also

### Providing predictions

protocol IntentPredictionConfiguration

An interface that provides the configuration for a single prediction.

enum IntentPredictionsBuilder

A result builder that allows you to declaratively describe the predictions for an app intent.

