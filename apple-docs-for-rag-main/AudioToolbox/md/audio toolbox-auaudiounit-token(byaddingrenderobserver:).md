

- Audio Toolbox
- AUAudioUnit
-  token(byAddingRenderObserver:) 

Instance Method

# token(byAddingRenderObserver:)

Adds a block to be called on each render cycle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func token(byAddingRenderObserver observer: @escaping AURenderObserver) -> Int
```

## Parameters 

`observer`  

The block to call.

## Return Value

A token to be used when removing the observer.

## Discussion

The supplied block is called at the beginning and ending of each render cycle. It should not make any blocking calls.

This method is implemented in the AUAudioUnit base class and should not be overridden.

This version 3 method is bridged to the version 2 AudioUnitAddRenderNotify(_:_:_:) API.

## See Also

### Managing the Render Cycle

func allocateRenderResources() throws

Allocates resources required to render audio.

func deallocateRenderResources()

Deallocates resources required to render audio.

func reset()

Resets transitory rendering state to its initial state.

var renderResourcesAllocated: Bool

Determines whether the audio unit has allocated render resources.

var renderBlock: AURenderBlock

The block that hosts use to ask the audio unit to render audio.

var scheduleParameterBlock: AUScheduleParameterBlock

The block that hosts use to schedule parameters.

var maximumFramesToRender: AUAudioFrameCount

The maximum number of frames that the audio unit can render at once.

func removeRenderObserver(Int)

Removes an observer block previously added to the render cycle.

typealias AURenderObserver

A block called when an audio unit renders audio.

