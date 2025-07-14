

- Audio Toolbox
- AUAudioUnit
-  deallocateRenderResources() 

Instance Method

# deallocateRenderResources()

Deallocates resources required to render audio.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func deallocateRenderResources()
```

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

Hosts should call this after finishing rendering. Subclasses should call the superclass implementation.

This version 3 method is bridged to the version 2 AudioUnitUninitialize(_:) API.

## See Also

### Managing the Render Cycle

func allocateRenderResources() throws

Allocates resources required to render audio.

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

func token(byAddingRenderObserver: AURenderObserver) -> Int

Adds a block to be called on each render cycle.

func removeRenderObserver(Int)

Removes an observer block previously added to the render cycle.

typealias AURenderObserver

A block called when an audio unit renders audio.

