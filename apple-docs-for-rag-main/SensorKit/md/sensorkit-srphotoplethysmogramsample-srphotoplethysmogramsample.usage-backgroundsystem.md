

- SensorKit
- SRPhotoplethysmogramSample
- SRPhotoplethysmogramSample.Usage
-  backgroundSystem 

Type Property

# backgroundSystem

A reading taken by the system in the background.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
static let backgroundSystem: SRPhotoplethysmogramSample.Usage
```

## Discussion

The system takes this reading while performing various heart features on watchOS — such as background blood oxygen, atrial fibrillation (AFib), and low-cardio notifications.

## See Also

### Getting the reading method

static let foregroundHeartRate: SRPhotoplethysmogramSample.Usage

A heart rate reading that a person takes while using an app.

static let deepBreathing: SRPhotoplethysmogramSample.Usage

A deep breathing sensor reading that a person takes while using an app.

static let foregroundBloodOxygen: SRPhotoplethysmogramSample.Usage

A blood oxygen reading that a person takes while using an app.

