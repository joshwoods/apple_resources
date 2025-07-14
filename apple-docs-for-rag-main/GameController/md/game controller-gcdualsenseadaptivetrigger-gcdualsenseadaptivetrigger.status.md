

- Game Controller
- GCDualSenseAdaptiveTrigger
-  GCDualSenseAdaptiveTrigger.Status 

Enumeration

# GCDualSenseAdaptiveTrigger.Status

The possible states of an adaptive trigger.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
enum Status
```

## Topics

### Statuses

case unknown

The trigger status is unknown.

case feedbackNoLoad

The trigger is in feedback mode, but isn’t applying the resistive load.

case feedbackLoadApplied

The trigger is in feedback mode and is applying the resistive load.

case weaponReady

The trigger is in weapon mode and ready to fire, but isn’t applying the resistive load.

case weaponFiring

The trigger is in weapon mode, firing, and is applying the resistive load.

case weaponFired

The trigger is in weapon mode, has fired, and has stopped applying the resistive load.

case vibrationNotVibrating

The trigger is in vibration mode, but isn’t vibrating.

case vibrationIsVibrating

The trigger is in vibration mode and is vibrating.

case slopeFeedbackReady

The trigger is in slope mode, but isn’t applying the resistive load.

case slopeFeedbackApplyingLoad

The trigger is in slope mode, and is applying the resistive load.

case slopeFeedbackFinished

The trigger is in slope mode, and stopped applying the resistive load.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking the status

var status: GCDualSenseAdaptiveTrigger.Status

The current status of the adaptive trigger and whether it’s applying effects.

