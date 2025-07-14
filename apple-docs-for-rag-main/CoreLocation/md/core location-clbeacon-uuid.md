

- Core Location
- CLBeacon
-  uuid 

Instance Property

# uuid

The UUID that the observed beacon transmitted.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
var uuid: UUID { get }
```

## Mentioned in 

Determining the proximity to an iBeacon device

## Discussion

The UUID is the most significant beacon identity characteristic. Multiple beacon can transmit the same UUID.

## See Also

### Getting the beacon identity

var major: NSNumber

The major value that the observed beacon transmitted.

var minor: NSNumber

The minor value that the observed beacon transmitted.

var proximityUUID: UUID

The proximity ID of the beacon.

Deprecated

