

- Audio Toolbox
- AUAudioUnit
-  renderBlock 

Instance Property

# renderBlock

The block that hosts use to ask the audio unit to render audio.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var renderBlock: AURenderBlock { get }
```

## Mentioned in 

Migrating Your Audio Unit Host to the AUv3 API

## Discussion

Before invoking an audio unit’s rendering functionality, a host should fetch this block and cache the result. The block can then be called from a realtime context without the possibility of blocking and causing an overload at the Core Audio HAL level.

This block will call a subclass’s internalRenderBlock implementation, providing all realtime events scheduled for the current render time interval, bracketed by calls to any render observers. Subclasses should override their internalRenderBlock implementation, not this property.

This version 3 property is bridged to the version 2 AudioUnitRender(_:_:_:_:_:_:) API.

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

