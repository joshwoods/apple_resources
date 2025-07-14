

- Create ML Components
- HumanBodyActionPeriodPredictor
-  HumanBodyActionPeriodPredictor.Output 

Type Alias

# HumanBodyActionPeriodPredictor.Output

The output type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Output = [HumanBodyActionPeriodPredictor.Prediction]
```

## See Also

### Performing the transformation

func applied(to: [Pose], eventHandler: EventHandler?) async throws -> [HumanBodyActionPeriodPredictor.Prediction]

Predicts human body action periods from an array of poses.

typealias Input

The input type.

struct Prediction

A human body action period prediction.

