

- Kernel
- Hardware Families
- Audio
-  IOAudioEngine 

Class

# IOAudioEngine

Abstract base class for a single audio audio / I/O engine.

macOS 10.1+

``` source
class IOAudioEngine : IOService
```

## Overview

An IOAudioEngine is defined by a single I/O engine to transfer data to or from one or more sample buffers. Each sample buffer is represented by a single IOAudioStream instance. A single IOAudioEngine must contain at least one IOAudioStream, but has no upper limit on the number of IOAudioStreams it may contain. An IOAudioEngine instance may contain both input and output IOAudioStreams.

An audio driver must subclass IOAudioEngine in order to provide certain services. An IOAudioEngine subclass must start and stop the I/O engine when requested. The I/O engine should be continuously running and loop around from end to beginning. While the audio engine is running, it must take a timestamp as the sample buffer(s) wrap around and start at the beginning. The CoreAudio.framework uses the timestamp to calculate the exact position of the audio engine. An IOAudioEngine subclass must implement getCurrentSampleFrame() to provide a sample position on demand. Finally, an IOAudioEngine subclass must provide clipping and format conversion routines to go to/from the CoreAudio.framework's native float format.

If multiple stream formats or sample rates are allowed, the IOAudioEngine subclass must provide support for changing the hardware when a format or sample rate is changed.

There are several attributes associated with a single IOAudioEngine:

The IOAudioEngine superclass provides a shared status buffer that contains all of the dynamic pieces of information about the audio engine (type IOAudioEngineStatus). It runs an erase process on all of the output streams. The erase head is used to zero out the mix and sample buffers after the samples have been played. Additionally, the IOAudioEngine superclass handles the communication with the CoreAudio.framework and makes the decision to start and stop the audio engine when it detects it is in use.

In order for an audio device to play back or record sound, an IOAudioEngine subclass must be created. The subclass must initialize all of the necessary hardware resources to prepare for starting the audio I/O engine. It typically will perform these tasks in the initHardware() method. A subclass may also implement a stop() method which is called as the driver is being torn down. This is typically called in preparation of removing the device from the system for removable devices.

In addition to initializing the necessary hardware, there are a number of other tasks an IOAudioEngine must do during initHardware(). It must create the necessary IOAudioStream objects to match the device capabilities. Each IOAudioStream must be added using addAudioStream(). It also should create the IOAudioControls needed to control the various attributes of the audio engine: output volume, mute, input gain, input selection, analog passthru. To do that, addDefaultAudioControl() should be called with each IOAudioControl to be attached to the IOAudioEngine. In order to provide for proper synchronization, the latency of the audio engine should be specified with setSampleLatency(). This value represents the latency between the timestamp taken at the beginning of the buffer and when the audio is actually played (or recorded) by the device. If a device is block based or if there is a need to keep the CoreAudio.framework a certain number of samples ahead of (or behind for input) the I/O head, that value should be specified using setSampleOffset(). If this is not specified the CoreAudio.framework may attempt to get as close to the I/O head as possible.

The following fields in the shared IOAudioEngineStatus struct must be maintained by the subclass implementation:

  &lt;t>  fCurrentLoopCount - the number of times the sample buffer has wrapped around to the beginning
  &lt;t>  fLastLoopTime - timestamp of the most recent time that the I/O engine looped back to the
  beginning of the sample buffer

It is critically important that the fLastLoopTime field be as accurate as possible. It is the basis for the entire timer and synchronization mechanism used by the audio system.

At init time, the IOAudioEngine subclass must call setNumSampleFramesPerBuffer() to indicate how large each of the sample buffers are (measured in sample frames). Within a single IOAudioEngine, all sample buffers must be the same size and be running at the same sample rate. If different buffers/streams can be run at different rates, separate IOAudioEngines should be used. The IOAudioEngine subclass must also call setSampleRate() at init time to indicate the starting sample rate of the device.

## Topics

### Miscellaneous

addAudioStream

Adds an IOAudioStream to the audio engine.

addTimer

Enables the timer event for the audio engine.

clearAllSampleBuffers

Zeros out all of the sample and mix buffers associated with the IOAudioEngine

clientClosed

Called automatically when a user client closes its connection to the audio engine.

convertInputSamplesVBR

Override this method if you want to return a different number of sample frames than was requested.

createDictionaryFromSampleRate

Generates a dictionary matching the given sample rate.

createSampleRateFromDictionary

Generates a sample rate from an OSDictionary.

eraseOutputSamples

This function allows for the actual erasing of the mix and sample buffer to be overridden by a child class.

free

Frees all of the resources allocated by the IOAudioEngine.

getAttributeForConnection

Generic method to retrieve some attribute of the audio engine, specific to one connection.

getCommandGate

Returns the IOCommandGate for this IOAudioEngine.

getCurrentSampleFrame

Gets the current sample frame from the IOAudioEngine subclass.

getRunEraseHead

Returns true if the audio engine will run the erase head when the audio engine is running.

getSampleRate

Returns the sample rate of the IOAudioEngine in samples per second.

getState

Returns the current state of the IOAudioEngine.

getStatus

Returns a pointer to the shared status buffer.

getTimerInterval

Gets the timer interval for use by the timer event.

getWorkLoop

Returns the IOWorkLoop for the driver.

init

Performs initialization of a newly allocated IOAudioEngine.

initHardware

This function is called by start() to provide a convenient place for the subclass to perform its hardware initialization.

initKeys

Generates the OSSymbols with the keys.

newUserClient

Requests a new user client object for this service.

performAudioEngineStart

Called to start the audio I/O engine

performAudioEngineStop

Called to stop the audio I/O engine

performErase

Performs erase head processing.

performFlush

Performs the flush operation.

registerService

Called when this audio engine is ready to begin vending services.

removeTimer

Disables the timer event for the audio engine.

resetStatusBuffer

Resets the status buffer to its default values.

setAttributeForConnection

Generic method to set some attribute of the audio engine, specific to one connection.

setClockDomain

Sets a property that CoreAudio uses to determine how devices are synchronized. If an audio device can tell that it is synchronized to another engine, it should set this value to that engine's clock domain. If an audio device can be a primary clock, it may publish its own clock domain for other devices to use.

setClockIsStable

This function sets a flag that CoreAudio uses to select its sample rate tracking algorithm. Set this to TRUE unless that results in dropped audio. If the driver is experiencing unexplained dropouts setting this FALSE might help.

setInputSampleOffset

set the offset CoreAudio will read from off the current read pointer

setMixClipOverhead

Used to tell IOAudioFamily when the watchdog timer must fire by.

setOutputSampleOffset

set the offset CoreAudio will write at off the current write pointer

setRunEraseHead

Tells the audio engine whether or not to run the erase head.

setSampleLatency

Sets the sample latency for the audio engine.

setSampleRate

Records the sample rate of the audio engine.

setState

Indicates that the audio engine is in the specified state.

start(IOService *)

A simple cover function for start(IOService \*, IOAudioDevice \*) that assumes the provider is the IOAudioDevice.

start(IOService *, IOAudioDevice *)

Standard IOKit start() routine called to start an IOService.

startAudioEngine

Starts the audio I/O engine.

stop

Stops the service and prepares for the driver to be terminated.

stopAudioEngine

Stops the audio I/O engine.

timerCallback

A static method used as a callback for the IOAudioDevice timer services.

timerFired

Indicates the timer has fired.

### Constants

gSampleRateWholeNumberKey

gSampleRateFractionKey

### Instance Variables

workLoop

userClients

status

state

sampleRate

runEraseHead

outputStreams

numSampleFramesPerBuffer

numErasesPerBuffer

numActiveUserClients

isRegistered

inputStreams

deviceStartedAudioEngine

defaultAudioControls

configurationChangeInProgress

commandGate

audioEngineStopPosition

audioDevice

### Instance Methods

- addAudioStreamDeprecated

- addDefaultAudioControlDeprecated

- addTimerDeprecated

- addUserClientDeprecated

- beginConfigurationChangeDeprecated

- calculateSampleTimeoutDeprecated

- calculateSampleTimeoutHiRes

- cancelConfigurationChangeDeprecated

- clearAllSampleBuffersDeprecated

- clientClosedDeprecated

- clipOutputSamplesDeprecated

- completeConfigurationChangeDeprecated

- convertInputSamplesDeprecated

- convertInputSamplesVBRDeprecated

- createUserClientDeprecated

- createUserClientDeprecated

- decrementActiveUserClientsDeprecated

- detachAudioStreamsDeprecated

- detachUserClientsDeprecated

- driverDesiresHiResSampleIntervals

- eraseOutputSamplesDeprecated

- freeDeprecated

- getAttributeForConnectionDeprecated

- getAudioStreamDeprecated

- getBytesInInputBufferArrayDescriptorDeprecated

- getBytesInOutputBufferArrayDescriptorDeprecated

- getCommandGate

- getCurrentSampleFrame

- getGlobalUniqueIDDeprecated

- getLocalUniqueIDDeprecated

- getLoopCountAndTimeStampDeprecated

- getMetaClass

- getNearestStartTimeDeprecated

- getNextStreamIDDeprecated

- getNumSampleFramesPerBufferDeprecated

- getRunEraseHeadDeprecated

- getSampleRateDeprecated

- getStateDeprecated

- getStatusDeprecated

- getStatusDescriptorDeprecated

- getStreamForIDDeprecated

- getTimerIntervalDeprecated

- getWorkLoop

- hardwareSampleRateChangedDeprecated

- incrementActiveUserClientsDeprecated

- initDeprecated

- initHardwareDeprecated

- lockAllStreamsDeprecated

- mixOutputSamplesDeprecated

- newUserClientDeprecated

- newUserClientDeprecated

- pauseAudioEngineDeprecated

- performAudioEngineStartDeprecated

- performAudioEngineStopDeprecated

- performEraseDeprecated

- performFlushDeprecated

- performFormatChangeDeprecated

- performFormatChangeDeprecated

- registerServiceDeprecated

- removeAllDefaultAudioControlsDeprecated

- removeDefaultAudioControlDeprecated

- removeTimerDeprecated

- removeUserClientDeprecated

- resetClipPositionDeprecated

- resetStatusBufferDeprecated

- resumeAudioEngineDeprecated

- sendFormatChangeNotificationDeprecated

- sendNotificationDeprecated

- setAttributeForConnectionDeprecated

- setAudioDeviceDeprecated

- setClockDomainDeprecated

- setClockIsStableDeprecated

- setDescriptionDeprecated

- setIndexDeprecated

- setInputSampleLatencyDeprecated

- setInputSampleOffsetDeprecated

- setMixClipOverheadDeprecated

- setNumSampleFramesPerBufferDeprecated

- setOutputSampleLatencyDeprecated

- setOutputSampleOffsetDeprecated

- setRunEraseHeadDeprecated

- setSampleLatencyDeprecated

- setSampleOffsetDeprecated

- setSampleRateDeprecated

- setStateDeprecated

- setWorkLoopOnAllAudioControlsDeprecated

- startDeprecated

- startDeprecated

- startAudioEngineDeprecated

- startClientDeprecated

- stopDeprecated

- stopAudioEngineDeprecated

- stopClientDeprecated

- stopEngineAtPositionDeprecated

- takeTimeStampDeprecated

- timerFiredDeprecated

- unlockAllStreamsDeprecated

- updateChannelNumbersDeprecated

- useHiResSampleInterval

- waitForEngineResume

### Type Methods

+ addUserClientActionDeprecated

+ createDictionaryFromSampleRateDeprecated

+ createSampleRateFromDictionaryDeprecated

+ detachUserClientsActionDeprecated

+ initKeysDeprecated

+ lockStreamForIODeprecated

+ removeUserClientActionDeprecated

+ setCommandGateUsageDeprecated

+ timerCallbackDeprecated

+ unlockStreamForIODeprecated

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOAudioLevelControl

IOAudioSelectorControl

IOAudioToggleControl

IOAudioControl

Represents any controllable attribute of an IOAudioDevice.

IOAudioStream

This class wraps a single sample buffer in an audio driver.

IOAudioPort

Represents a logical or physical port or functional unit in an audio device.

