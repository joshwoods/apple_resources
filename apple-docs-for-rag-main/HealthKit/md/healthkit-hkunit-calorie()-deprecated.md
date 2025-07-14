

- HealthKit
- HKUnit
-  calorie() Deprecated

Type Method

# calorie()

Returns a HealthKit unit for measuring energy in calories.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
class func calorie() -> Self
```

Deprecated

To avoid confusion, use largeCalorie() or smallCalorie() instead.

## Return Value

A HealthKit unit for measuring energy in calories.

## See Also

### Constructing energy units

class func joule() -> Self

Returns a HealthKit unit for measuring energy in joules.

class func jouleUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring energy, using joule units with the provided prefix.

class func kilocalorie() -> Self

Returns a HealthKit unit for measuring energy in kilocalories.

class func largeCalorie() -> Self

Returns a HealthKit unit for measuring energy in large calories (Cal).

class func smallCalorie() -> Self

Returns a HealthKit unit for measuring energy in small calories (cal).

