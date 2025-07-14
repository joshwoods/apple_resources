

- Foundation
- Process
-  run(\_:arguments:terminationHandler:) 

Type Method

# run(\_:arguments:terminationHandler:)

Creates and runs a task with a specified executable and arguments.

macOS 10.13+

``` source
class func run(
    _ url: URL,
    arguments: [String],
    terminationHandler: ((Process) -> Void)? = nil
) throws -> Process
```

## Parameters 

`url`  

The URL for the executable.

`arguments`  

An array of `NSString` objects that supplies the arguments to the task. If `arguments` is `nil`, the system raises an `NSInvalidArgumentException`.

`terminationHandler`  

The system invokes this completion block when the task has completed.

## Return Value

An initialized `NSTask` object with the environment of the current process.

## See Also

### Creating and Initializing

init()

Returns an initialized process object with the environment of the current process.

