

- Audio Toolbox
- AUAudioUnit
-  scheduleParameterBlock 

Instance Property

# scheduleParameterBlock

The block that hosts use to schedule parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var scheduleParameterBlock: AUScheduleParameterBlock { get }
```

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

As with the render block, a host should fetch this block before beginning to render, if it intends to schedule parameters.

The block is safe to call from any thread context, including realtime audio render threads. Subclasses should not override this; it is implemented in the base class and will schedule the events to be provided to the internalRenderBlock implementation

This version 3 property is bridged to the version 2 AudioUnitScheduleParameters(_:_:_:) API.

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

var maximumFramesToRender: AUAudioFrameCount

The maximum number of frames that the audio unit can render at once.

func token(byAddingRenderObserver: AURenderObserver) -> Int

Adds a block to be called on each render cycle.

func removeRenderObserver(Int)

Removes an observer block previously added to the render cycle.

typealias AURenderObserver

A block called when an audio unit renders audio.

