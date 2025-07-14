

- VisionKit
- ImageAnalysisInteraction
-  didMove(to:) 

Instance Method

# didMove(to:)

Performs an action after the view adds or removes the interaction from its interaction array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
final func didMove(to view: UIView?)
```

## Parameters 

`view`  

The view that owns and contains the interaction in its interaction array.

## See Also

### Responding to view events

func willMove(to: UIView?)

Performs an action before the view adds or removes the interaction from its interaction array.

