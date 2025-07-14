

- Core Audio
- AudioHardwareObject
-  setPropertyData(address:qualifier:data:) 

Instance Method

# setPropertyData(address:qualifier:data:)

macOS 15.0+

``` source
func setPropertyData(
    address: AudioObjectPropertyAddress,
    qualifier: Data? = nil,
    data: inout Data
) async throws
```

