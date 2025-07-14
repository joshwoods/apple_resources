

- Foundation
- ProcessInfo
-  operatingSystemVersion 

Instance Property

# operatingSystemVersion

The version of the operating system on which the process is executing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var operatingSystemVersion: OperatingSystemVersion { get }
```

## See Also

### Getting Host Information

var hostName: String

The name of the host computer on which the process is executing.

var operatingSystemVersionString: String

A string containing the version of the operating system on which the process is executing.

func isOperatingSystemAtLeast(OperatingSystemVersion) -> Bool

Returns a Boolean value indicating whether the version of the operating system on which the process is executing is the same or later than the given version.

func operatingSystem() -> Int

Returns a constant to indicate the operating system on which the process is executing.

Deprecated

func operatingSystemName() -> String

Returns a string containing the name of the operating system on which the process is executing.

Deprecated

