

- Foundation
- Process
-  launchPath Deprecated

Instance Property

# launchPath

Sets the receiver’s executable.

macOS 10.0–15.4Deprecated

``` source
var launchPath: String? { get set }
```

Deprecated

Use executableURL instead.

## Parameters 

`path`  

The path to the executable.

## See Also

### Deprecated

class func launchedProcess(launchPath: String, arguments: [String]) -> Process

Creates and launches a task with a specified executable and arguments.

Deprecated

var currentDirectoryPath: String

Sets the current directory for the receiver.

Deprecated

func launch()

Launches the task represented by the receiver.

Deprecated

