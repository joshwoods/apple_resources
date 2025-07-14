

- IOBluetooth
- IOBluetoothOBEXSession
-  isSessionTargetAMac() 

Instance Method

# isSessionTargetAMac()

Tells whether the target device is a Mac by checking its service record.

macOS

``` source
func isSessionTargetAMac() -> Bool
```

## Return Value

TRUE only if device service record has Mac entry, FALSE for all else.

## Discussion

Tells whether the target device is a Mac by checking its service record.

