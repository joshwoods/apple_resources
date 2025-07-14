

- Quartz
- IKScannerDeviceViewDelegate
-  scannerDeviceView(\_:didEncounterError:) 

Instance Method

# scannerDeviceView(\_:didEncounterError:)

Invoked whenever the scanner encounters an error.

macOS 10.6+

``` source
optional func scannerDeviceView(
    _ scannerDeviceView: IKScannerDeviceView!,
    didEncounterError error: (any Error)!
)
```

## Parameters 

`scannerDeviceView`  

The scanner device that sent the message.

`error`  

The error.

