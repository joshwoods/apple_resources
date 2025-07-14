

- Core Haptics
-  CHHapticEventParameter 

Class

# CHHapticEventParameter

A static parameter value that represents a single property of the haptic pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class CHHapticEventParameter
```

## Overview

Event parameters specify values for haptics associated with the event. For example, an intensity event parameter determines how intense the haptic feels when it fires. Event parameters are static; they don’t change over the course of the pattern. To change a parameter value after a haptic has started playing, use a CHHapticDynamicParameter to make an immediate change, or a CHHapticParameterCurve to transition smoothly.

When you send a dynamic parameter to the haptic pattern, its value changes immediately, at the specified time. When you send a parameter curve instead, the value changes gradually according to the type of curve you specified.

## Topics

### Creating an Event Parameter

init(parameterID: CHHapticEvent.ParameterID, value: Float)

Creates a haptic event parameter from its ID and value.

struct ParameterID

An identifier for an event parameter.

### Specifying an Event Parameter’s Value

var parameterID: CHHapticEvent.ParameterID

The haptic parameter ID indicating what type of parameter the current event represents.

var value: Float

The value of the parameter.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Programmatic haptics

Delivering Rich App Experiences with Haptics

Enhance your app’s experience by incorporating haptic and sound feedback into key interactive moments.

Playing Collision-Based Haptic Patterns

Play a custom haptic pattern whose strength depends on an object’s collision speed.

Updating Continuous and Transient Haptic Parameters in Real Time

Generate continuous and transient haptic patterns in response to user touch.

class CHHapticEvent

An object that describes a single haptic or audio event.

class CHHapticDynamicParameter

A value that you send to a haptic pattern player to alter a property value during playback.

class CHHapticParameterCurve

A curve that you send to a haptic pattern player to alter a property value gradually during playback.

