

- Foundation
- ProcessInfo
-  operatingSystem() Deprecated

Instance Method

# operatingSystem()

Returns a constant to indicate the operating system on which the process is executing.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func operatingSystem() -> Int
```

Deprecated

Use operatingSystemVersion or isOperatingSystemAtLeast(_:) instead

## Return Value

Operating system identifier. See Constants for a list of possible values. In macOS, it’s `NSMACHOperatingSystem`.

## See Also

### Getting Host Information

var hostName: String

The name of the host computer on which the process is executing.

var operatingSystemVersionString: String

A string containing the version of the operating system on which the process is executing.

var operatingSystemVersion: OperatingSystemVersion

The version of the operating system on which the process is executing.

func isOperatingSystemAtLeast(OperatingSystemVersion) -> Bool

Returns a Boolean value indicating whether the version of the operating system on which the process is executing is the same or later than the given version.

func operatingSystemName() -> String

Returns a string containing the name of the operating system on which the process is executing.

Deprecated

