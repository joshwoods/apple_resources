

- Foundation
- Process
-  launch() Deprecated

Instance Method

# launch()

Launches the task represented by the receiver.

macOS 10.0–15.4Deprecated

``` source
func launch()
```

Deprecated

Use run() instead.

## Discussion

Raises an `NSInvalidArgumentException` if the launch path has not been set or is invalid or if it fails to create a process.

## See Also

### Related Documentation

func waitUntilExit()

Blocks the process until the receiver is finished.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

### Deprecated

class func launchedProcess(launchPath: String, arguments: [String]) -> Process

Creates and launches a task with a specified executable and arguments.

Deprecated

var currentDirectoryPath: String

Sets the current directory for the receiver.

Deprecated

var launchPath: String?

Sets the receiver’s executable.

Deprecated

