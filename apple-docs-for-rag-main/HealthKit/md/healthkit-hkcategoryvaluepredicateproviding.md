

- HealthKit
-  HKCategoryValuePredicateProviding 

Protocol

# HKCategoryValuePredicateProviding

A protocol for objects that produce predicates that match category value samples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOSwatchOS 9.0+

``` source
protocol HKCategoryValuePredicateProviding : Hashable, RawRepresentable
```

## Topics

### Creating predicates

static func predicateForSamples(NSComparisonPredicate.Operator, value: Self) -> NSPredicate

Returns a predicate that checks a category sample’s value.

static func predicateForSamples(equalTo: Set&lt;Self>) -> NSPredicate

Returns a predicate that checks whether a category sample is equal to the provided set of values.

## Relationships

### Inherits From

- Equatable
- Hashable
- RawRepresentable

### Conforming Types

- HKCategoryValue
- HKCategoryValueAppetiteChanges
- HKCategoryValueAppleStandHour
- HKCategoryValueAppleWalkingSteadinessEvent
- HKCategoryValueCervicalMucusQuality
- HKCategoryValueContraceptive
- HKCategoryValueEnvironmentalAudioExposureEvent
- HKCategoryValueHeadphoneAudioExposureEvent
- HKCategoryValueLowCardioFitnessEvent
- HKCategoryValueMenstrualFlow
- HKCategoryValueOvulationTestResult
- HKCategoryValuePregnancyTestResult
- HKCategoryValuePresence
- HKCategoryValueProgesteroneTestResult
- HKCategoryValueSeverity
- HKCategoryValueSleepAnalysis
- HKCategoryValueVaginalBleeding

## See Also

### Creating category sample predicates

class func predicateForCategorySamples(with: NSComparisonPredicate.Operator, value: Int) -> NSPredicate

Returns a predicate that checks a category sample’s value.

Deprecated

