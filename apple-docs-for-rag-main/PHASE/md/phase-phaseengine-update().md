

- PHASE
- PHASEEngine
-  update() 

Instance Method

# update()

Processes app commands and increments framework processing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func update()
```

## Discussion

This function consumes the app’s API calls since the last update(), adjusts internal systems, objects, increments parameters, and invokes the app’s queued callbacks. An API call may require several update() invocations before the output device reflects the call’s results.

The framework ignores calls to this function for engines with `updateMode` set to PHASEEngine.UpdateMode.automatic; for more more information, see init(updateMode:).

Note

The frequency that the app calls this function doesn’t change the speed by which PHASE plays audio in real time.

### Update an Engine Manually

On an engine configured for manual updates (PHASEEngine.UpdateMode.manual), call this function periodically to instruct the framework to process API calls and perform internal updates. Call update() at a rate that matches your app’s visuals or logic update rate for optimal performance:

- Apps that process graphics at 60 FPS can invoke update() in their display link callback.

- Rates in the range of 240Hz to 30Hz offer equivalent audio performance, however apps that actively change the parameters of playing audio achieve smoother interpolation at a higher rate.

- If a game skips frames due to long running graphics routines, an app can throttle update() calls to values less than 30Hz without affecting audio quality as long as the system isn’t overloaded.

This function offers thread safety for apps that intend to call update() off of the main thread.

## See Also

### Controlling and Inspecting Playback State

func pause()

Pauses all audio playback.

func start() throws

Starts or resumes all audio playback.

func stop()

Stops all audio playback.

var renderingState: PHASESoundEvent.RenderingState

The status of the engine’s audio playback.

