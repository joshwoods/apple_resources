

- HealthKit
- HKCategoryTypeIdentifier
-  sleepAnalysis 

Type Property

# sleepAnalysis

A category sample type for sleep analysis information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
static let sleepAnalysis: HKCategoryTypeIdentifier
```

## Mentioned in 

Saving data to HealthKit

## Discussion

These samples use values from the HKCategoryValueSleepAnalysis enum.

For best results when analyzing sleep samples, it’s recommended that you use HKMetadataKeyTimeZone to store time zone metadata with your sleep sample data.

## See Also

### Mindfulness and sleep

static let mindfulSession: HKCategoryTypeIdentifier

A category sample type for recording a mindful session.

static let appleSleepingWristTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the wrist temperature during sleep.

enum HKAppleSleepingBreathingDisturbancesClassification

