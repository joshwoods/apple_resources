

- Foundation
- Process
-  currentDirectoryPath Deprecated

Instance Property

# currentDirectoryPath

Sets the current directory for the receiver.

macOS 10.0–15.4Deprecated

``` source
var currentDirectoryPath: String { get set }
```

Deprecated

Use currentDirectoryURL instead.

## Parameters 

`path`  

The current directory for the task.

## Discussion

If this method isn’t used, the current directory is inherited from the process that created the receiver. This method raises an `NSInvalidArgumentException` if the receiver has already been launched.

## See Also

### Deprecated

class func launchedProcess(launchPath: String, arguments: [String]) -> Process

Creates and launches a task with a specified executable and arguments.

Deprecated

var launchPath: String?

Sets the receiver’s executable.

Deprecated

func launch()

Launches the task represented by the receiver.

Deprecated

