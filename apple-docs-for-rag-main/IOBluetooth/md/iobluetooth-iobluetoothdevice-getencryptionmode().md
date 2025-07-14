

- IOBluetooth
- IOBluetoothDevice
-  getEncryptionMode() 

Instance Method

# getEncryptionMode()

Get the encryption mode for the baseband connection.

macOS

``` source
func getEncryptionMode() -> BluetoothHCIEncryptionMode
```

## Return Value

Returns the encryption mode for the baseband connection. If no baseband connection is present, kEncryptionDisabled is returned.

## Discussion

This method only returns a valid result if a baseband connection is present (-isConnected returns TRUE).

