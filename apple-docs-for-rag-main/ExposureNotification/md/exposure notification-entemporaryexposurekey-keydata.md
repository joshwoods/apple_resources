

- Exposure Notification
- ENTemporaryExposureKey
-  keyData 

Instance Property

# keyData

The temporary exposure key information.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var keyData: Data { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

## See Also

### Exposure Criteria

var transmissionRiskLevel: ENRiskLevel

The risk of transmission associated with the person a key came from.

var rollingPeriod: ENIntervalNumber

The length of time that this key is valid.

var rollingStartNumber: ENIntervalNumber

A number that indicates when a key’s rolling period started.

typealias ENIntervalNumber

A number assigned to each 10-minute window shared between all devices participating in the protocol.

