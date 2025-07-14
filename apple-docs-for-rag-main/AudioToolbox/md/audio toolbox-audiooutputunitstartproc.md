

- Audio Toolbox
-  AudioOutputUnitStartProc 

Type Alias

# AudioOutputUnitStartProc

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioOutputUnitStartProc = (UnsafeMutableRawPointer) -> OSStatus
```

## See Also

### Starting and Stopping Output

func AudioOutputUnitStart(AudioUnit) -> OSStatus

Starts an I/O audio unit, which in turn starts the audio unit processing graph that it is connected to.

func AudioOutputUnitStop(AudioUnit) -> OSStatus

Stops an I/O audio unit, which in turn stops the audio unit processing graph that it is connected to.

typealias AudioOutputUnitStopProc

