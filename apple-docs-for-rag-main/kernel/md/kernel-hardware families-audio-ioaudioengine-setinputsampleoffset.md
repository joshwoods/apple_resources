

- Kernel
- Hardware Families
- Audio
- IOAudioEngine
-  setInputSampleOffset 

# setInputSampleOffset

set the offset CoreAudio will read from off the current read pointer

``` source
virtual void setInputSampleOffset(
 UInt32numSamples); 
```

## Parameters 

`numSamples`  

size of offset in sample

## See Also

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

