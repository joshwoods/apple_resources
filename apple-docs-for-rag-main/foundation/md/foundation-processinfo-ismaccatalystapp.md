

- Foundation
- ProcessInfo
-  isMacCatalystApp 

Instance Property

# isMacCatalystApp

A Boolean value that indicates whether the process originated as an iOS app and runs on macOS.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isMacCatalystApp: Bool { get }
```

## Discussion

The value of this property is true when the process is:

- A Mac app built with Mac Catalyst, or an iOS app running on Apple silicon.

- Running on a Mac.

Frameworks that support iOS and macOS use this property to determine if the process is a Mac app built with Mac Catalyst. To conditionally compile source code intended to run only in macOS, use `#if targetEnvironment(macCatalyst)` (or `#if TARGET_OS_MACCATALYST` in Objective-C) instead.

Note

To distinguish between an iOS app running on Apple silicon and a Mac app built with Mac Catalyst, use the isiOSAppOnMac property.

## See Also

### Accessing Process Information

var arguments: [String]

Array of strings with the command-line arguments for the process.

var environment: [String : String]

The variable names (keys) and their values in the environment from which the process was launched.

var globallyUniqueString: String

Global unique identifier for the process.

var isiOSAppOnMac: Bool

A Boolean value that indicates whether the process is an iPhone or iPad app running on a Mac.

var processIdentifier: Int32

The identifier of the process (often called process ID).

var processName: String

The name of the process.

