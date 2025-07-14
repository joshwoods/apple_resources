

- Create ML Components
- HumanBodyActionPeriodPredictor
-  HumanBodyActionPeriodPredictor.Prediction 

Structure

# HumanBodyActionPeriodPredictor.Prediction

A human body action period prediction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Prediction
```

## Topics

### Creating a prediction

init(period: Float, periodicity: Float)

Creates a human body action period prediction.

### Getting the properties

var period: Float

The duration of a human body action measured in frames.

var periodicity: Float

A score that indicates whether this frame contributes to a periodic human body action.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Performing the transformation

func applied(to: [Pose], eventHandler: EventHandler?) async throws -> [HumanBodyActionPeriodPredictor.Prediction]

Predicts human body action periods from an array of poses.

typealias Input

The input type.

typealias Output

The output type.

