

- IOBluetooth
-  IOBluetoothUnpackDataList(\_:\_:\_:\_:) 

Function

# IOBluetoothUnpackDataList(\_:\_:\_:\_:)

macOS

``` source
func IOBluetoothUnpackDataList(
    _ inBufferSize: Int,
    _ inBuffer: UnsafeRawPointer!,
    _ inFormat: UnsafePointer!,
    _ inArgs: CVaListPointer
) -> Int
```

## See Also

### Functions

func IOBluetoothNSStringFromDeviceAddressColon(UnsafePointer&lt;BluetoothDeviceAddress>!) -> String!

func IOBluetoothPackDataList(UnsafeMutableRawPointer!, UnsafePointer&lt;CChar>!, CVaListPointer) -> Int

