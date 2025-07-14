

- Quartz
- QCView
-  autostartsRendering() Deprecated

Instance Method

# autostartsRendering()

Checks whether the view is set to start rendering automatically.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func autostartsRendering() -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

Returns true if the view is set to start rendering automatically when the view is put on screen.

## See Also

### Managing Rendering

func startRendering() -> Bool

Starts rendering the composition that is in the view.

Deprecated

func isRendering() -> Bool

Checks whether a composition is rendering in the view.

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

