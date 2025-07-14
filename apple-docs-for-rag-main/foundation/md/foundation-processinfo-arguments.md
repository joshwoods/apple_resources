

- Foundation
- ProcessInfo
-  arguments 

Instance Property

# arguments

Array of strings with the command-line arguments for the process.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var arguments: [String] { get }
```

## Discussion

This array contains all the information passed in the `argv` array, including the executable name in the first element.

## See Also

### Accessing Process Information

var environment: [String : String]

The variable names (keys) and their values in the environment from which the process was launched.

var globallyUniqueString: String

Global unique identifier for the process.

var isMacCatalystApp: Bool

A Boolean value that indicates whether the process originated as an iOS app and runs on macOS.

var isiOSAppOnMac: Bool

A Boolean value that indicates whether the process is an iPhone or iPad app running on a Mac.

var processIdentifier: Int32

The identifier of the process (often called process ID).

var processName: String

The name of the process.

