

- Foundation
- Process
-  launchedProcess(launchPath:arguments:) Deprecated

Type Method

# launchedProcess(launchPath:arguments:)

Creates and launches a task with a specified executable and arguments.

macOS 10.0–15.4Deprecated

``` source
class func launchedProcess(
    launchPath path: String,
    arguments: [String]
) -> Process
```

Deprecated

Use run(_:arguments:terminationHandler:) instead.

## Parameters 

`path`  

The path to the executable.

`arguments`  

An array of `NSString` objects that supplies the arguments to the task. If `arguments` is `nil`, an `NSInvalidArgumentException` is raised.

## Return Value

An initialized `NSTask` object with the supplied `arguments`.

## Discussion

The task inherits its environment from the process that invokes this method.

The `NSTask` object converts both `path` and the strings in `arguments` to appropriate C-style strings (using fileSystemRepresentation) before passing them to the task via `argv[])` . The strings in `arguments` don’t undergo shell expansion, so you don’t need to do special quoting, and shell variables, such as `$PWD`, aren’t resolved.

## See Also

### Related Documentation

init()

Returns an initialized process object with the environment of the current process.

### Deprecated

var currentDirectoryPath: String

Sets the current directory for the receiver.

Deprecated

var launchPath: String?

Sets the receiver’s executable.

Deprecated

func launch()

Launches the task represented by the receiver.

Deprecated

