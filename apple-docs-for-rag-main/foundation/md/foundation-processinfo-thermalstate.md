

- Foundation
- ProcessInfo
-  thermalState 

Instance Property

# thermalState

The current thermal state of the system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var thermalState: ProcessInfo.ThermalState { get }
```

## Discussion

At higher thermal states your app should reduce usage of system resources. For more information, see ProcessInfo.ThermalState.

