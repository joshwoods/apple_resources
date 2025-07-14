

- ImageCaptureCore
- ICScannerDeviceDelegate
-  scannerDeviceDidBecomeAvailable(\_:) 

Instance Method

# scannerDeviceDidBecomeAvailable(\_:)

Tells the client when another client closes the current open session on the scanner.

macOS 10.4+

``` source
optional func scannerDeviceDidBecomeAvailable(_ scanner: ICScannerDevice)
```

## Discussion

Scanners require exclusive access. Only one client can open a session on a scanner at a time. The scanner is available if it does not have a session opened by another client. Attempting to open a session on a scanner that already has an open session for another client will result in an error.

To open a session on a scanner as soon as it is available, implement this method and call requestOpenSession() in the method body.

