

- Foundation
- ProcessInfo
-  operatingSystemVersionString 

Instance Property

# operatingSystemVersionString

A string containing the version of the operating system on which the process is executing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var operatingSystemVersionString: String { get }
```

## Discussion

The operating system version string is human readable, localized, and is appropriate for displaying to the user. This string is *not* appropriate for parsing.

## See Also

### Getting Host Information

var hostName: String

The name of the host computer on which the process is executing.

var operatingSystemVersion: OperatingSystemVersion

The version of the operating system on which the process is executing.

func isOperatingSystemAtLeast(OperatingSystemVersion) -> Bool

Returns a Boolean value indicating whether the version of the operating system on which the process is executing is the same or later than the given version.

func operatingSystem() -> Int

Returns a constant to indicate the operating system on which the process is executing.

Deprecated

func operatingSystemName() -> String

Returns a string containing the name of the operating system on which the process is executing.

Deprecated

