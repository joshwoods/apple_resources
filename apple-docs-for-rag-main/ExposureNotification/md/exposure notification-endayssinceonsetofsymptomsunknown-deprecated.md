

- Exposure Notification
-  ENDaysSinceOnsetOfSymptomsUnknown Deprecated

Global Variable

# ENDaysSinceOnsetOfSymptomsUnknown

A value used when the number of days since onset of symptoms is unknown.

iOS 14.0–14.2DeprecatediPadOS 14.0–14.2DeprecatedMac Catalyst 14.0–14.2Deprecated

``` source
let ENDaysSinceOnsetOfSymptomsUnknown: Int
```

Deprecated

Server must provide keys with days_since_onset_of_symptoms set.

## Discussion

Important

This property is available in iOS 12.5, and in iOS 14.0 and later.

## See Also

### Configuring Infectiousness

var infectiousnessForDaysSinceOnsetOfSymptoms: [NSNumber : NSNumber]?

The mapping between the days since onset of symptoms to the degree of infectiousness.

var infectiousnessHighWeight: Double

The weight to apply for severe infectiousness.

var infectiousnessStandardWeight: Double

The weight to apply for mild infectiousness.

