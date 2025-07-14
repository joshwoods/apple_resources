

- HomeKit
-  HMCharacteristicTypeRemoteKey 

Global Variable

# HMCharacteristicTypeRemoteKey

The accessory remote control key.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let HMCharacteristicTypeRemoteKey: String
```

## Overview

`HMCharacteristicTypeRemoteKey` describes a mechanism to send control key presses to televisions. The handling of the key presses depend on the current active input source, or the application that is running. The corresponding value is one of the constants in the HMCharacteristicValueRemoteKey enumeration.

## Topics

### Values

enum HMCharacteristicValueRemoteKey

Values for the state of the remote.

## See Also

### Locks and openers

let HMCharacteristicTypeLockManagementAutoSecureTimeout: String

The automatic timeout for a lockable accessory that supports automatic lockout.

let HMCharacteristicTypeLockManagementControlPoint: String

A control that accepts vendor-specific actions for lock management.

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

