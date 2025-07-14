

- Audio Toolbox
-  AudioUnitRemoveRenderNotify(\_:\_:\_:) 

Function

# AudioUnitRemoveRenderNotify(\_:\_:\_:)

Unregisters a previously-registered render listener callback function.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioUnitRemoveRenderNotify(
    _ inUnit: AudioUnit,
    _ inProc: AURenderCallback,
    _ inProcUserData: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`inUnit`  

The audio unit that you no longer want to receive render notifications from.

`inProc`  

The callback function that you previously registered and are now unregistering.

`inProcUserData`  

The custom data that you provided when registering the callback function.

## Return Value

A result code.

## See Also

### Rendering the Audio

func AudioUnitRender(AudioUnit, UnsafeMutablePointer&lt;AudioUnitRenderActionFlags>?, UnsafePointer&lt;AudioTimeStamp>, UInt32, UInt32, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Initiates a rendering cycle for an audio unit.

func AudioUnitAddRenderNotify(AudioUnit, AURenderCallback, UnsafeMutableRawPointer?) -> OSStatus

Registers a callback to receive audio unit render notifications.

typealias AURenderCallback

Called by the system when an audio unit requires input samples, or before and after a render operation.

struct AudioUnitRenderActionFlags

Flags for configuring audio unit rendering.

