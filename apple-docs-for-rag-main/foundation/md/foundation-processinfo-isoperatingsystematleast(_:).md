

- Foundation
- ProcessInfo
-  isOperatingSystemAtLeast(\_:) 

Instance Method

# isOperatingSystemAtLeast(\_:)

Returns a Boolean value indicating whether the version of the operating system on which the process is executing is the same or later than the given version.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isOperatingSystemAtLeast(_ version: OperatingSystemVersion) -> Bool
```

## Parameters 

`version`  

The operating system version to test against.

## Return Value

true if the operating system on which the process is executing is the same or later than the given version; otherwise false.

## Discussion

This method accounts for major, minor, and update versions of the operating system.

## See Also

### Getting Host Information

var hostName: String

The name of the host computer on which the process is executing.

var operatingSystemVersionString: String

A string containing the version of the operating system on which the process is executing.

var operatingSystemVersion: OperatingSystemVersion

The version of the operating system on which the process is executing.

func operatingSystem() -> Int

Returns a constant to indicate the operating system on which the process is executing.

Deprecated

func operatingSystemName() -> String

Returns a string containing the name of the operating system on which the process is executing.

Deprecated

