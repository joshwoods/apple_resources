

- Core Location
- CLMonitor
- CLMonitor.BeaconIdentityCondition
-  init(uuid:) 

Initializer

# init(uuid:)

Creates a beacon identity condition with the UUID characteristic only, and wildcard values for the major and minor characteristics.

iOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
init(uuid: UUID)
```

## Parameters 

`uuid`  

The UUID that identifies the beacon.

## See Also

### Creating a beacon identity condition

init(uuid: UUID, major: UInt16)

Creates a beacon identity condition with UUID and major characteristics, and a wildcard for the minor characteristic.

init(uuid: UUID, major: UInt16, minor: UInt16)

Creates a beacon identity condition with UUID, and major and minor characteristics.

