

- Audio Toolbox
-  AudioOutputUnitStop(\_:) 

Function

# AudioOutputUnitStop(\_:)

Stops an I/O audio unit, which in turn stops the audio unit processing graph that it is connected to.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioOutputUnitStop(_ ci: AudioUnit) -> OSStatus
```

## Parameters 

`ci`  

The I/O audio unit to stop.

## Return Value

A result code.

## See Also

### Starting and Stopping Output

func AudioOutputUnitStart(AudioUnit) -> OSStatus

Starts an I/O audio unit, which in turn starts the audio unit processing graph that it is connected to.

typealias AudioOutputUnitStartProc

typealias AudioOutputUnitStopProc

