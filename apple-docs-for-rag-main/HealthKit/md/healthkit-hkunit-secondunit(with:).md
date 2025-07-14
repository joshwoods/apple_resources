

- HealthKit
- HKUnit
-  secondUnit(with:) 

Type Method

# secondUnit(with:)

Returns a HealthKit unit for measuring time, using second units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func secondUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring time based on seconds and the provided prefix.

## Discussion

This method is used to create prefixed versions of seconds. Common uses include creating millisecond units, as shown below.

- Swift
- Objective-C

```
let ms = HKUnit.secondUnitWithMetricPrefix(.Milli)
```

```
HKUnit *ms = [HKUnit secondUnitWithMetricPrefix:HKMetricPrefixMilli];
```

## See Also

### Constructing time units

class func second() -> Self

Returns a HealthKit unit for measuring time in seconds.

class func minute() -> Self

Returns a HealthKit unit for measuring time in minutes.

class func hour() -> Self

Returns a HealthKit unit for measuring time in hours.

class func day() -> Self

Returns a HealthKit unit for measuring time in days.

