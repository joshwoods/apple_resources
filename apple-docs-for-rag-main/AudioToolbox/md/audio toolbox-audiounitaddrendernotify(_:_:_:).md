

- Audio Toolbox
-  AudioUnitAddRenderNotify(\_:\_:\_:) 

Function

# AudioUnitAddRenderNotify(\_:\_:\_:)

Registers a callback to receive audio unit render notifications.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitAddRenderNotify(
    _ inUnit: AudioUnit,
    _ inProc: AURenderCallback,
    _ inProcUserData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you want to receive render notifications from.

`inProc`  

The callback that you are registering.

`inProcUserData`  

Custom data that you want to be sent to your callback. Use this, for example, to identify the render listener.

## Return Value

A result code.

## Discussion

The registered callback function is called both before the audio unit performs its render operations (when the render flag’s pre-render bit is set) and after the audio unit has completed its render operation (the render flag’s post-render bit is set).

The `inProc` and `inProcUserData` parameters are treated as a two-part identifier. To remove a render listener, you must pass both these values to the AudioUnitRemoveRenderNotify(_:_:_:) function.

## See Also

### Rendering the Audio

func AudioUnitRender(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Initiates a rendering cycle for an audio unit.

func AudioUnitRemoveRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Unregisters a previously-registered render listener callback function.

typealias AURenderCallback

Called by the system when an audio unit requires input samples, or before and after a render operation.

struct AudioUnitRenderActionFlags

Flags for configuring audio unit rendering.

