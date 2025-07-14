

- HealthKit
- HKUnit
-  siemenUnit(with:) 

Type Method

# siemenUnit(with:)

Returns a HealthKit unit for measuring electrical conductance, using siemen units with the provided prefix.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func siemenUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Return Value

A HealthKit unit for measuring electrical conductance based on siemens and the provided prefix.

## Discussion

This method is used to create prefixed versions of siemens. HealthKit often records electrodermal activity in microsiemens, as shown below.

- Swift
- Objective-C

```
let mcS = HKUnit.siemenUnitWithMetricPrefix(.Micro)
```

```
HKUnit *mcS = [HKUnit siemenUnitWithMetricPrefix:HKMetricPrefixMicro];
```

## See Also

### Constructing electrical conductance units

class func siemen() -> Self

Returns a HealthKit unit for measuring electrical conductance in siemens.

