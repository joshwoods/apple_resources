

- Audio Toolbox
-  AUParameter 

Class

# AUParameter

An object that represents a single audio unit parameter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUParameter
```

## Topics

### Querying Parameter Properties

var minValue: AUValue

The parameter’s minimum value.

var maxValue: AUValue

The parameter’s maximum value.

var unit: AudioUnitParameterUnit

The parameter’s unit of measurement.

var unitName: String?

The parameter’s localized unit name.

var flags: AudioUnitParameterOptions

The parameter’s characteristic details.

var address: AUParameterAddress

The parameter’s address.

var valueStrings: [String]?

The parameter’s localized value strings.

var dependentParameters: [NSNumber]?

Any other parameter’s whose values may change as a side effect of this parameter’s value changing.

### Managing Parameter Values

var value: AUValue

The parameter’s current value.

func setValue(AUValue, originator: AUParameterObserverToken?)

Sets the parameter’s value, avoiding redundant notifications to the originator.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64)

Sets the parameter’s value, preserving the host time of the gesture that initiated the change.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64, eventType: AUParameterAutomationEventType)

func string(fromValue: UnsafePointer&lt;AUValue>?) -> String

Gets the string representation of a parameter value.

func value(from: String) -> AUValue

Converts a string into a parameter value.

## Relationships

### Inherits From

- AUParameterNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Parameters

class AUParameterGroup

A parameter group object represents a group of related audio unit parameters.

class AUParameterNode

An object that represents a node in an audio unit’s parameter tree.

class AUParameterTree

An object that represents a top-level group node that contains all of an audio unit’s parameters.

