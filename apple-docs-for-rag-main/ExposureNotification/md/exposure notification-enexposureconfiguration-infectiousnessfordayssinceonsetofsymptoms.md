

- Exposure Notification
- ENExposureConfiguration
-  infectiousnessForDaysSinceOnsetOfSymptoms 

Instance Property

# infectiousnessForDaysSinceOnsetOfSymptoms

The mapping between the days since onset of symptoms to the degree of infectiousness.

iOS 12.5+iPadOS 12.5+Mac Catalyst 12.5+

``` source
var infectiousnessForDaysSinceOnsetOfSymptoms: [NSNumber : NSNumber]? { get set }
```

## Discussion

Important

This property is available in iOS 12.5, and in iOS 13.7 and later.

The dictionary key is the day since the onset of symptoms. The corresponding value is an ENInfectiousness value. When the day is not known, use ENDaysSinceOnsetOfSymptomsUnknown as the dictionary key, like this:

```
infectiousnessForDaysSinceOnsetOfSymptoms[ENDaysSinceOnsetOfSymptionsUnknown] = 
        infectiousnessHighWeight;
```

You can’t change this property more often than once per week. During development, you can remove this limitation by adding the test entitlement `com.apple.developer.exposure-notification-test` to your project.

Note

You must set this property when using the version 2 scoring algorithm.

## See Also

### Configuring Infectiousness

var infectiousnessHighWeight: Double

The weight to apply for severe infectiousness.

var infectiousnessStandardWeight: Double

The weight to apply for mild infectiousness.

let ENDaysSinceOnsetOfSymptomsUnknown: Int

A value used when the number of days since onset of symptoms is unknown.

Deprecated

