

- Core Audio
- AudioHardwareDevice
-  start(at:flags:IOProcID:) 

Instance Method

# start(at:flags:IOProcID:)

macOS 15.0+

``` source
func start(
    at time: AudioTimeStamp,
    flags: UInt32 = 0,
    IOProcID: AudioDeviceIOProcID? = nil
) throws -> AudioTimeStamp?
```

