

- Quartz
- QCCompositionPickerView
-  isAnimating() Deprecated

Instance Method

# isAnimating()

Returns whether or not the composition picker view is currently animating its composition.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func isAnimating() -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

true if a composition is animating in the composition picker view; false otherwise.

## See Also

### Managing Animation

func startAnimation(Any!)

Starts animating the composition in the composition picker view.

Deprecated

func stopAnimation(Any!)

Stops animating the composition that is currently animating in the composition picker view.

Deprecated

func setMaxAnimationFrameRate(Float)

Sets the maximum frame rate for animating compositions.

Deprecated

func maxAnimationFrameRate() -> Float

Retrieves the maximum frame rate for animating compositions.

Deprecated

