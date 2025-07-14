

- Audio Toolbox
-  AudioOutputUnitStart(\_:) 

Function

# AudioOutputUnitStart(\_:)

Starts an I/O audio unit, which in turn starts the audio unit processing graph that it is connected to.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func AudioOutputUnitStart(_ ci: AudioUnit) -> OSStatus
```

## Parameters 

`ci`  

The I/O audio unit to start.

## Return Value

A result code.

## See Also

### Starting and Stopping Output

func AudioOutputUnitStop(AudioUnit) -> OSStatus

Stops an I/O audio unit, which in turn stops the audio unit processing graph that it is connected to.

typealias AudioOutputUnitStartProc

typealias AudioOutputUnitStopProc

