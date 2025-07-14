

- Quartz
- QCCompositionPickerView
-  startAnimation(\_:) Deprecated

Instance Method

# startAnimation(\_:)

Starts animating the composition in the composition picker view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func startAnimation(_ sender: Any!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`sender`  

The object initiating the animation.

## See Also

### Managing Animation

func stopAnimation(Any!)

Stops animating the composition that is currently animating in the composition picker view.

Deprecated

func isAnimating() -> Bool

Returns whether or not the composition picker view is currently animating its composition.

Deprecated

func setMaxAnimationFrameRate(Float)

Sets the maximum frame rate for animating compositions.

Deprecated

func maxAnimationFrameRate() -> Float

Retrieves the maximum frame rate for animating compositions.

Deprecated

