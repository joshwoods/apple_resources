

- App Intents
-  IntentPredictionConfiguration 

Protocol

# IntentPredictionConfiguration

An interface that provides the configuration for a single prediction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol IntentPredictionConfiguration
```

## Topics

### Associated Types

associatedtype Intent : AppIntent

**Required**

## Relationships

### Conforming Types

- IntentPrediction
- TupleIntentPrediction

## See Also

### Providing predictions

static var predictionConfiguration: Self.Prediction

A collection of predictions the system can use when it suggests the app intent.

**Required**

enum IntentPredictionsBuilder

A result builder that allows you to declaratively describe the predictions for an app intent.

