

- VisionKit
- ImageAnalysisInteraction
-  willMove(to:) 

Instance Method

# willMove(to:)

Performs an action before the view adds or removes the interaction from its interaction array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
final func willMove(to view: UIView?)
```

## Parameters 

`view`  

The view that owns and contains the interaction in its interaction array.

## See Also

### Responding to view events

func didMove(to: UIView?)

Performs an action after the view adds or removes the interaction from its interaction array.

