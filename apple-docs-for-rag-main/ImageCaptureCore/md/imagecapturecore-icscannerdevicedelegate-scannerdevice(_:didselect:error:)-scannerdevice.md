

- ImageCaptureCore
- ICScannerDeviceDelegate
-  scannerDevice(\_:didSelect:error:) 

Instance Method

# scannerDevice(\_:didSelect:error:)

Tells the client when a functional unit is selected on the scanner.

macOS 10.4+

``` source
optional func scannerDevice(
    _ scanner: ICScannerDevice,
    didSelect functionalUnit: ICScannerFunctionalUnit,
    error: (any Error)?
)
```

## Discussion

A functional unit is selected immediately after the scanner instantiates and in response to calling requestSelect(_:).

