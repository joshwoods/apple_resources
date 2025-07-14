

- Quartz
- QCCompositionPickerView
-  setMaxAnimationFrameRate(\_:) Deprecated

Instance Method

# setMaxAnimationFrameRate(\_:)

Sets the maximum frame rate for animating compositions.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setMaxAnimationFrameRate(_ maxFPS: Float)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`maxFPS`  

A frame rate in frames per second. Pass `0.0` to specify no limit to the maximum value.

## See Also

### Managing Animation

func startAnimation(Any!)

Starts animating the composition in the composition picker view.

Deprecated

func stopAnimation(Any!)

Stops animating the composition that is currently animating in the composition picker view.

Deprecated

func isAnimating() -> Bool

Returns whether or not the composition picker view is currently animating its composition.

Deprecated

func maxAnimationFrameRate() -> Float

Retrieves the maximum frame rate for animating compositions.

Deprecated

