

- Audio Toolbox
-  AURenderCallback 

Type Alias

# AURenderCallback

Called by the system when an audio unit requires input samples, or before and after a render operation.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AURenderCallback = (UnsafeMutableRawPointer, UnsafeMutablePointer, UnsafePointer, UInt32, UInt32, UnsafeMutablePointer?) -> OSStatus
```

## Parameters 

`inRefCon`  

Custom data that you provided when registering your callback with the audio unit.

`ioActionFlags`  

Flags used to describe more about the context of this call (pre or post in the notify case for instance).

`inTimeStamp`  

The timestamp associated with this call of audio unit render.

`inBusNumber`  

The bus number associated with this call of audio unit render.

`inNumberFrames`  

The number of sample frames that will be represented in the audio data in the provided ioData parameter.

`ioData`  

The AudioBufferList that will be used to contain the rendered or provided audio data.

## Return Value

A result code.

## Discussion

If you named your callback function `MyAURenderCallback`, you would declare it like this:

### Discussion

You can use this callback function with both the audio unit render notification API (see the AudioUnitAddRenderNotify(_:_:_:) function) and the render input callback (see the `kAudioUnitProperty_SetRenderCallback` property).

As a notification listener, the system invokes this callback before and after an audio unit’s render operations.

As a render operation input callback, it is invoked when an audio unit requires input samples for the input bus that the callback is attached to.

## See Also

### Rendering the Audio

func AudioUnitRender(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Initiates a rendering cycle for an audio unit.

func AudioUnitAddRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit render notifications.

func AudioUnitRemoveRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered render listener callback function.

struct AudioUnitRenderActionFlags

Flags for configuring audio unit rendering.

