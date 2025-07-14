

- Create ML Components
- HumanBodyActionPeriodPredictor
-  HumanBodyActionPeriodPredictor.Input 

Type Alias

# HumanBodyActionPeriodPredictor.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Input = [Pose]
```

## See Also

### Performing the transformation

func applied(to: [Pose], eventHandler: EventHandler?) async throws -> [HumanBodyActionPeriodPredictor.Prediction]

Predicts human body action periods from an array of poses.

typealias Output

The output type.

struct Prediction

A human body action period prediction.

