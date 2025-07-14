

- Foundation
- Process
-  init() 

Initializer

# init()

Returns an initialized process object with the environment of the current process.

Mac Catalyst 13.0+macOS 10.0+

``` source
init()
```

## Return Value

An initialized process object with the environment of the current process.

## Discussion

If you need to modify the environment of a process, use alloc and init, and then set up the environment before launching the new process. Otherwise, just use the class method run(_:arguments:terminationHandler:) to create and run the process.

## See Also

### Creating and Initializing

class func run(URL, arguments: [String], terminationHandler: ((Process) -> Void)?) throws -> Process

Creates and runs a task with a specified executable and arguments.

