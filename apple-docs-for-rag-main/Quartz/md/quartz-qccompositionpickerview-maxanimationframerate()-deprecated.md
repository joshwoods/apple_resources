

- Quartz
- QCCompositionPickerView
-  maxAnimationFrameRate() Deprecated

Instance Method

# maxAnimationFrameRate()

Retrieves the maximum frame rate for animating compositions.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func maxAnimationFrameRate() -> Float
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The maximum frame rate.

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

func setMaxAnimationFrameRate(Float)

Sets the maximum frame rate for animating compositions.

Deprecated

