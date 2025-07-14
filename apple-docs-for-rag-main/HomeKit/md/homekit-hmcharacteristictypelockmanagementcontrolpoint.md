

- HomeKit
-  HMCharacteristicTypeLockManagementControlPoint 

Global Variable

# HMCharacteristicTypeLockManagementControlPoint

A control that accepts vendor-specific actions for lock management.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeLockManagementControlPoint: String
```

## Discussion

The corresponding write-only value takes data in a format specified by the accessory’s manufacturer.

## See Also

### Locks and openers

let HMCharacteristicTypeLockManagementAutoSecureTimeout: String

The automatic timeout for a lockable accessory that supports automatic lockout.

let HMCharacteristicTypeLockMechanismLastKnownAction: String

The last known action of the locking mechanism.

let HMCharacteristicTypeLockPhysicalControls: String

The lock’s physical control state.

let HMCharacteristicTypeMotionDetected: String

An indicator of whether the accessory has detected motion.

let HMCharacteristicTypeCurrentLockMechanismState: String

The current state of the locking mechanism.

let HMCharacteristicTypeTargetLockMechanismState: String

The target state for the locking mechanism.

let HMCharacteristicTypeRemoteKey: String

The accessory remote control key.

