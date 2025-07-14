

- HealthKit
- HKUnit
-  count() 

Type Method

# count()

Returns a HealthKit unit for measuring counts.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func count() -> Self
```

## Return Value

A HealthKit unit for measuring counts.

## Discussion

Count units are used to represent raw scalar values. They are often used to represent the number of times an event occurs—for example, the number of steps the user has taken or the number of times the user has used his or her inhaler. They can also be used as part of a compound unit—for example, the beats portion of beats per minute. Even though count and percent units are both scalar units, you cannot convert between them.

Note

In HealthKit quantities, count values are stored using `double` values, even though they are often interpreted as integers.

## See Also

### Constructing scalar units

class func percent() -> Self

Returns a HealthKit unit for measuring percentages.

