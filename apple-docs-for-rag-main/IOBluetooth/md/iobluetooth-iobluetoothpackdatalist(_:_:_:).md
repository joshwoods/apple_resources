

- IOBluetooth
-  IOBluetoothPackDataList(\_:\_:\_:) 

Function

# IOBluetoothPackDataList(\_:\_:\_:)

macOS

``` source
func IOBluetoothPackDataList(
    _ ioBuffer: UnsafeMutableRawPointer!,
    _ inFormat: UnsafePointer!,
    _ inArgs: CVaListPointer
) -> Int
```

## See Also

### Functions

func IOBluetoothNSStringFromDeviceAddressColon(UnsafePointer&lt;BluetoothDeviceAddress>!) -> String!

func IOBluetoothUnpackDataList(Int, UnsafeRawPointer!, UnsafePointer&lt;CChar>!, CVaListPointer) -> Int

