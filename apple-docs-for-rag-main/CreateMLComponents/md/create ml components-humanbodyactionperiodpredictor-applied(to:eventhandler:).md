

- Create ML Components
- HumanBodyActionPeriodPredictor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Predicts human body action periods from an array of poses.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: [Pose],
    eventHandler: EventHandler? = nil
) async throws -> [HumanBodyActionPeriodPredictor.Prediction]
```

## Parameters 

`input`  

An async sequence of pose windows.

`eventHandler`  

An event handler.

## Return Value

An async sequence of predictions.

## See Also

### Performing the transformation

typealias Input

The input type.

typealias Output

The output type.

struct Prediction

A human body action period prediction.

