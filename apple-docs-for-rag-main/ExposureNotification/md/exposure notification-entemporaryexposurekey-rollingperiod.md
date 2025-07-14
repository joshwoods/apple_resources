

- Exposure Notification
- ENTemporaryExposureKey
-  rollingPeriod 

Instance Property

# rollingPeriod

The length of time that this key is valid.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var rollingPeriod: ENIntervalNumber { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

The value of this property is the number of 10-minute windows between key rolling.

## See Also

### Exposure Criteria

var transmissionRiskLevel: ENRiskLevel

The risk of transmission associated with the person a key came from.

var keyData: Data

The temporary exposure key information.

var rollingStartNumber: ENIntervalNumber

A number that indicates when a key’s rolling period started.

typealias ENIntervalNumber

A number assigned to each 10-minute window shared between all devices participating in the protocol.

