

- Foundation
- ProcessInfo
-  isiOSAppOnMac 

Instance Property

# isiOSAppOnMac

A Boolean value that indicates whether the process is an iPhone or iPad app running on a Mac.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isiOSAppOnMac: Bool { get }
```

## Discussion

The value of this property is true only when the process is an iOS app running on a Mac. The value of the property is false for all other apps on the Mac, including Mac apps built using Mac Catalyst. The property is also false for processes running on platforms other than macOS.

## See Also

### Accessing Process Information

var arguments: [String]

Array of strings with the command-line arguments for the process.

var environment: [String : String]

The variable names (keys) and their values in the environment from which the process was launched.

var globallyUniqueString: String

Global unique identifier for the process.

var isMacCatalystApp: Bool

A Boolean value that indicates whether the process originated as an iOS app and runs on macOS.

var processIdentifier: Int32

The identifier of the process (often called process ID).

var processName: String

The name of the process.

