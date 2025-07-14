

- Foundation
- ProcessInfo
-  processInfo 

Type Property

# processInfo

Returns the process information agent for the process.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var processInfo: ProcessInfo { get }
```

## Return Value

Shared process information agent for the process.

## Discussion

An ProcessInfo object is created the first time this method is invoked, and that same object is returned on each subsequent invocation.

