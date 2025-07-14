

- Exposure Notification
-  ENIntervalNumber 

Type Alias

# ENIntervalNumber

A number assigned to each 10-minute window shared between all devices participating in the protocol.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
typealias ENIntervalNumber = UInt32
```

## Discussion

These shared intervals of time derive from timestamps in UNIX Epoch Time.

`ENIntervalNumber(Timestamp) ← Timestamp / (60×10)`

## See Also

### Exposure Criteria

var transmissionRiskLevel: ENRiskLevel

The risk of transmission associated with the person a key came from.

var rollingPeriod: ENIntervalNumber

The length of time that this key is valid.

var keyData: Data

The temporary exposure key information.

var rollingStartNumber: ENIntervalNumber

A number that indicates when a key’s rolling period started.

