

- Quartz
- QCView
-  setAutostartsRendering(\_:) Deprecated

Instance Method

# setAutostartsRendering(\_:)

Sets whether the composition that is in the view starts rendering automatically when the view is put on the screen.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setAutostartsRendering(_ flag: Bool)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`flag`  

Pass true to enable autostart mode; false otherwise.

## See Also

### Managing Rendering

func startRendering() -> Bool

Starts rendering the composition that is in the view.

Deprecated

func isRendering() -> Bool

Checks whether a composition is rendering in the view.

Deprecated

func autostartsRendering() -> Bool

Checks whether the view is set to start rendering automatically.

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

