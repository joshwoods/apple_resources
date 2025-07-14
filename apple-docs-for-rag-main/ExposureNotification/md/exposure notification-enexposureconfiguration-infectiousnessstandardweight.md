

- Exposure Notification
- ENExposureConfiguration
-  infectiousnessStandardWeight 

Instance Property

# infectiousnessStandardWeight

The weight to apply for mild infectiousness.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var infectiousnessStandardWeight: Double { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

The range of this value is 0-250%

## See Also

### Configuring Infectiousness

var infectiousnessForDaysSinceOnsetOfSymptoms: [NSNumber : NSNumber]?

The mapping between the days since onset of symptoms to the degree of infectiousness.

var infectiousnessHighWeight: Double

The weight to apply for severe infectiousness.

let ENDaysSinceOnsetOfSymptomsUnknown: Int

A value used when the number of days since onset of symptoms is unknown.

Deprecated

