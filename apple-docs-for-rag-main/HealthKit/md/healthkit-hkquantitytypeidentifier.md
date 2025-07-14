

- HealthKit
-  HKQuantityTypeIdentifier 

Structure

# HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct HKQuantityTypeIdentifier
```

## Overview

To create an HKQuantityType instance, pass an HKQuantityTypeIdentifier value to the quantityType(forIdentifier:) method.

## Topics

### Activity

static let stepCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of steps the user has taken.

static let distanceWalkingRunning: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved by walking or running.

static let runningGroundContactTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the runner’s foot is in contact with the ground while running.

static let runningPower: HKQuantityTypeIdentifier

A quantity sample type that measures the rate of work required for the runner to maintain their speed.

static let runningSpeed: HKQuantityTypeIdentifier

A quantity sample type that measures the runner’s speed.

static let runningStrideLength: HKQuantityTypeIdentifier

A quantity sample type that measures the distance covered by a single step while running.

static let runningVerticalOscillation: HKQuantityTypeIdentifier

A quantity sample type measuring pelvis vertical range of motion during a single running stride.

static let distanceCycling: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved by cycling.

static let pushCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of pushes that the user has performed while using a wheelchair.

static let distanceWheelchair: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved using a wheelchair.

static let swimmingStrokeCount: HKQuantityTypeIdentifier

A quantity sample type that measures the number of strokes performed while swimming.

static let distanceSwimming: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has moved while swimming.

static let distanceDownhillSnowSports: HKQuantityTypeIdentifier

A quantity sample type that measures the distance the user has traveled while skiing or snowboarding.

static let basalEnergyBurned: HKQuantityTypeIdentifier

A quantity sample type that measures the resting energy burned by the user.

static let activeEnergyBurned: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of active energy the user has burned.

static let flightsClimbed: HKQuantityTypeIdentifier

A quantity sample type that measures the number flights of stairs that the user has climbed.

static let nikeFuel: HKQuantityTypeIdentifier

A quantity sample type that measures the number of NikeFuel points the user has earned.

static let appleExerciseTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the user spent exercising.

static let appleMoveTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the user has spent performing activities that involve full-body movements during the specified day.

static let appleStandTime: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of time the user has spent standing.

static let vo2Max: HKQuantityTypeIdentifier

A quantity sample that measures the maximal oxygen consumption during exercise.

### Body measurements

static let height: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s height.

static let bodyMass: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s weight.

static let bodyMassIndex: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s body mass index.

static let leanBodyMass: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s lean body mass.

static let bodyFatPercentage: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s body fat percentage.

static let waistCircumference: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s waist circumference.

static let appleSleepingWristTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the wrist temperature during sleep.

### Reproductive health

static let basalBodyTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the user’s basal body temperature.

### Hearing

static let environmentalAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure to sounds in the environment.

static let headphoneAudioExposure: HKQuantityTypeIdentifier

A quantity sample type that measures audio exposure from headphones.

### Vital signs

static let heartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate.

static let restingHeartRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s resting heart rate.

static let walkingHeartRateAverage: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s heart rate while walking.

static let heartRateVariabilitySDNN: HKQuantityTypeIdentifier

A quantity sample type that measures the standard deviation of heartbeat intervals.

static let heartRateRecoveryOneMinute: HKQuantityTypeIdentifier

A quantity sample that records the reduction in heart rate from the peak exercise rate to the rate one minute after exercising ended.

static let atrialFibrillationBurden: HKQuantityTypeIdentifier

A quantity type that measures an estimate of the percentage of time a person’s heart shows signs of atrial fibrillation (AFib) while wearing Apple Watch.

static let oxygenSaturation: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s oxygen saturation.

static let bodyTemperature: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s body temperature.

static let bloodPressureDiastolic: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s diastolic blood pressure.

static let bloodPressureSystolic: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s systolic blood pressure.

static let respiratoryRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s respiratory rate.

### Lab and test results

static let bloodGlucose: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s blood glucose level.

static let electrodermalActivity: HKQuantityTypeIdentifier

A quantity sample type that measures electrodermal activity.

static let forcedExpiratoryVolume1: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of air that can be forcibly exhaled from the lungs during the first second of a forced exhalation.

static let forcedVitalCapacity: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of air that can be forcibly exhaled from the lungs after taking the deepest breath possible.

static let inhalerUsage: HKQuantityTypeIdentifier

A quantity sample type that measures the number of puffs the user takes from their inhaler.

static let insulinDelivery: HKQuantityTypeIdentifier

A quantity sample that measures the amount of insulin delivered.

static let numberOfTimesFallen: HKQuantityTypeIdentifier

A quantity sample type that measures the number of times the user fell.

static let peakExpiratoryFlowRate: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s maximum flow rate generated during a forceful exhalation.

static let peripheralPerfusionIndex: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s peripheral perfusion index.

### Mindfulness and Sleep

static let appleSleepingWristTemperature: HKQuantityTypeIdentifier

A quantity sample type that records the wrist temperature during sleep.

### Nutrition

static let dietaryBiotin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of biotin (vitamin B7) consumed.

static let dietaryCaffeine: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of caffeine consumed.

static let dietaryCalcium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of calcium consumed.

static let dietaryCarbohydrates: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of carbohydrates consumed.

static let dietaryChloride: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of chloride consumed.

static let dietaryCholesterol: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of cholesterol consumed.

static let dietaryChromium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of chromium consumed.

static let dietaryCopper: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of copper consumed.

static let dietaryEnergyConsumed: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of energy consumed.

static let dietaryFatMonounsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of monounsaturated fat consumed.

static let dietaryFatPolyunsaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of polyunsaturated fat consumed.

static let dietaryFatSaturated: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of saturated fat consumed.

static let dietaryFatTotal: HKQuantityTypeIdentifier

A quantity sample type that measures the total amount of fat consumed.

static let dietaryFiber: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of fiber consumed.

static let dietaryFolate: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of folate (folic acid) consumed.

static let dietaryIodine: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of iodine consumed.

static let dietaryIron: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of iron consumed.

static let dietaryMagnesium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of magnesium consumed.

static let dietaryManganese: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of manganese consumed.

static let dietaryMolybdenum: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of molybdenum consumed.

static let dietaryNiacin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of niacin (vitamin B3) consumed.

static let dietaryPantothenicAcid: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of pantothenic acid (vitamin B5) consumed.

static let dietaryPhosphorus: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of phosphorus consumed.

static let dietaryPotassium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of potassium consumed.

static let dietaryProtein: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of protein consumed.

static let dietaryRiboflavin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of riboflavin (vitamin B2) consumed.

static let dietarySelenium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of selenium consumed.

static let dietarySodium: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of sodium consumed.

static let dietarySugar: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of sugar consumed.

static let dietaryThiamin: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of thiamin (vitamin B1) consumed.

static let dietaryVitaminA: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin A consumed.

static let dietaryVitaminB12: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of cyanocobalamin (vitamin B12) consumed.

static let dietaryVitaminB6: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of pyridoxine (vitamin B6) consumed.

static let dietaryVitaminC: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin C consumed.

static let dietaryVitaminD: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin D consumed.

static let dietaryVitaminE: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin E consumed.

static let dietaryVitaminK: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of vitamin K consumed.

static let dietaryWater: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of water consumed.

static let dietaryZinc: HKQuantityTypeIdentifier

A quantity sample type that measures the amount of zinc consumed.

### Alcohol consumption

static let bloodAlcoholContent: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s blood alcohol content.

static let numberOfAlcoholicBeverages: HKQuantityTypeIdentifier

A quantity sample type that measures the number of standard alcoholic drinks that the user has consumed.

### Mobility

static let appleWalkingSteadiness: HKQuantityTypeIdentifier

A quantity sample type that measures the steadiness of the user’s gait.

static let sixMinuteWalkTestDistance: HKQuantityTypeIdentifier

A quantity sample type that stores the distance a user can walk during a six-minute walk test.

static let walkingSpeed: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s average speed when walking steadily over flat ground.

static let walkingStepLength: HKQuantityTypeIdentifier

A quantity sample type that measures the average length of the user’s step when walking steadily over flat ground.

static let walkingAsymmetryPercentage: HKQuantityTypeIdentifier

A quantity sample type that measures the percentage of steps in which one foot moves at a different speed than the other when walking on flat ground.

static let walkingDoubleSupportPercentage: HKQuantityTypeIdentifier

A quantity sample type that measures the percentage of time when both of the user’s feet touch the ground while walking steadily over flat ground.

static let stairAscentSpeed: HKQuantityTypeIdentifier

A quantity sample type measuring the user’s speed while climbing a flight of stairs.

static let stairDescentSpeed: HKQuantityTypeIdentifier

A quantity sample type measuring the user’s speed while descending a flight of stairs.

### UV exposure

static let uvExposure: HKQuantityTypeIdentifier

A quantity sample type that measures the user’s exposure to UV radiation.

### Diving

static let underwaterDepth: HKQuantityTypeIdentifier

A quantity sample that records a person’s depth underwater.

static let waterTemperature: HKQuantityTypeIdentifier

A quantity sample that records the water temperature.

### Initializers

init(rawValue: String)

Returns a newly initialized quantity type identifier using the provided string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating quantity types

class func quantityType(forIdentifier: HKQuantityTypeIdentifier) -> HKQuantityType?

Returns the shared quantity type for the provided identifier.

