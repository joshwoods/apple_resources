

- Exposure Notification
- ENExposureConfiguration
-  transmissionRiskWeight 

Instance Property

# transmissionRiskWeight

The weight assigned to a score for the affected user’s estimated risk of transmission.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var transmissionRiskWeight: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.5 and later.

This weight parameter is not used.

## See Also

### Weight Configuration

var attenuationWeight: Double

The weight assigned to a score for the Bluetooth signal strength.

var daysSinceLastExposureWeight: Double

The weight assigned to a score for the days since the user’s exposure.

var durationWeight: Double

The weight assigned to a score for the duration of the user’s exposure.

