

- Core Location
- CLMonitor
- CLMonitor.BeaconIdentityCondition
-  init(uuid:major:) 

Initializer

# init(uuid:major:)

Creates a beacon identity condition with UUID and major characteristics, and a wildcard for the minor characteristic.

iOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
init(
    uuid: UUID,
    major: UInt16
)
```

## Parameters 

`uuid`  

The UUID that identifies the beacon.

`major`  

The CLBeaconMajorValue that represents the beacon’s major value.

## See Also

### Creating a beacon identity condition

init(uuid: UUID)

Creates a beacon identity condition with the UUID characteristic only, and wildcard values for the major and minor characteristics.

init(uuid: UUID, major: UInt16, minor: UInt16)

Creates a beacon identity condition with UUID, and major and minor characteristics.

