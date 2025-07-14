

- HealthKit
- HKUnit
-  percent() 

Type Method

# percent()

Returns a HealthKit unit for measuring percentages.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func percent() -> Self
```

## Return Value

A HealthKit unit for measuring percentages.

## Discussion

Percent measures a value between 0.0 and 1.0. HealthKit uses percent units when measuring body fat percentage, oxygen saturation, blood alcohol content, and similar values. Even though count and percent units are both scalar units, you cannot convert between them.

## See Also

### Constructing scalar units

class func count() -> Self

Returns a HealthKit unit for measuring counts.

