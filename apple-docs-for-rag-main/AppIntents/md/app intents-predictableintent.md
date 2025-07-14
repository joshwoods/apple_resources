

- App Intents
-  PredictableIntent 

Protocol

# PredictableIntent

An interface that allows the system to suggest the app intent to someone in the future using predictions you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PredictableIntent : AppIntent
```

## Topics

### Providing predictions

static var predictionConfiguration: Self.Prediction

A collection of predictions the system can use when it suggests the app intent.

**Required**

protocol IntentPredictionConfiguration

An interface that provides the configuration for a single prediction.

enum IntentPredictionsBuilder

A result builder that allows you to declaratively describe the predictions for an app intent.

### Associated Types

associatedtype Prediction : IntentPredictionConfiguration

**Required**

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

## See Also

### Intent predictions

struct IntentPrediction

A prediction for a specific app intent that the system might display to someone when it’s relevant.

