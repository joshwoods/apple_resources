

- HomeKit
-  HMCharacteristicWriteAction 

Class

# HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMCharacteristicWriteAction where TargetValueType : NSCopying
```

## Overview

Action sets are instances of HMActionSet.

## Topics

### New Methods

init(characteristic: HMCharacteristic, targetValue: TargetValueType)

Initialize a characteristic write action with a specified characteristic and target value.

var characteristic: HMCharacteristic

The characteristic whose value is to be written by the action.

var targetValue: TargetValueType

The value that will be written to the characteristic when the action is executed.

func updateTargetValue(TargetValueType, completionHandler: ((any Error)?) -> Void)

Updates the target value.

## Relationships

### Inherits From

- HMAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Defining the associated actions

var actions: Set&lt;HMAction>

Set of actions in the action set.

func addAction(HMAction, completionHandler: HMErrorBlock)

Adds an action to the action set.

func removeAction(HMAction, completionHandler: HMErrorBlock)

Removes an action from the action set.

class HMAction

An abstract base class for actions in HomeKit.

