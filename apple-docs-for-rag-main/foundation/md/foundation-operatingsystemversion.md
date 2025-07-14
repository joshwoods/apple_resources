

- Foundation
-  OperatingSystemVersion 

Structure

# OperatingSystemVersion

A structure that contains version information about the currently executing operating system, including major, minor, and patch version numbers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct OperatingSystemVersion
```

## Overview

Use the ProcessInfo property operatingSystemVersion to fetch an instance of this type. You can also pass this type to isOperatingSystemAtLeast(_:) to determine whether the current operating system version is the same or later than the given value.

## Topics

### Creating an Operating System Version

init()

Creates an empty operating system version.

init(majorVersion: Int, minorVersion: Int, patchVersion: Int)

Creates an operating system version with the provided values.

### Version Components

var majorVersion: Int

The major release number, such as 10 in version 10.9.3.

var minorVersion: Int

The minor release number, such as 9 in version 10.9.3.

var patchVersion: Int

The update release number, such as 3 in version 10.9.3.

var majorVersion: Int

The major release number, such as 10 in version 10.9.3.

var minorVersion: Int

The minor release number, such as 9 in version 10.9.3.

var patchVersion: Int

The update release number, such as 3 in version 10.9.3.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Constants

struct ActivityOptions

Option flags used with beginActivity(options:reason:) and performActivity(options:reason:using:).

enum ThermalState

Values used to indicate the system’s thermal state.

Anonymous

The following constants are provided by the `NSProcessInfo` class as return values for operatingSystem().

