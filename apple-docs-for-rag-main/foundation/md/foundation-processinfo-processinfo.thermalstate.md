

- Foundation
- ProcessInfo
-  ProcessInfo.ThermalState 

Enumeration

# ProcessInfo.ThermalState

Values used to indicate the system’s thermal state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum ThermalState
```

## Overview

These values are used by the ProcessInfo class as return values for thermalState.

For information about testing your app under different thermal states, see Test under adverse device conditions.

## Topics

### Constants

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case serious

The thermal state is high.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case serious

The thermal state is high.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

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

### Constants

struct OperatingSystemVersion

A structure that contains version information about the currently executing operating system, including major, minor, and patch version numbers.

struct ActivityOptions

Option flags used with beginActivity(options:reason:) and performActivity(options:reason:using:).

Anonymous

The following constants are provided by the `NSProcessInfo` class as return values for operatingSystem().

