

- Quartz
- QCView
-  isRendering() Deprecated

Instance Method

# isRendering()

Checks whether a composition is rendering in the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func isRendering() -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

Returns true if a composition is rendering in the view; false otherwise.

## See Also

### Managing Rendering

func startRendering() -> Bool

Starts rendering the composition that is in the view.

Deprecated

func autostartsRendering() -> Bool

Checks whether the view is set to start rendering automatically.

Deprecated

func setAutostartsRendering(Bool)

Sets whether the composition that is in the view starts rendering automatically when the view is put on the screen.

Deprecated

func stopRendering()

Stops rendering the composition that is in the view.

Deprecated

func pauseRendering()

Pauses rendering in the view.

Deprecated

func isPausedRendering() -> Bool

Returns whether or not the rendering in the view is paused.

Deprecated

func resumeRendering()

Resumes rendering a paused composition.

Deprecated

