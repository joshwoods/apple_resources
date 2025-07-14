

- Foundation
- Process
-  standardError 

Instance Property

# standardError

The standard error for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var standardError: Any? { get set }
```

## Parameters 

`file`  

The standard error for the receiver, which can be either an FileHandle or an Pipe object.

## Discussion

If `file` is an `NSPipe` object, launching the receiver automatically closes the write end of the pipe in the current task. Don’t create a handle for the pipe and pass that as the argument, or the system won’t automatically close the write end of the pipe.

If this method isn’t used, the standard error is inherited from the process that created the receiver. This method raises an `NSInvalidArgumentException` if the system has lauched the receiver.

## See Also

### Configuring

var arguments: [String]?

The command arguments that the system uses to launch the executable.

var currentDirectoryURL: URL?

The current directory for the receiver.

var environment: [String : String]?

The environment for the receiver.

var executableURL: URL?

The receiver’s executable.

var qualityOfService: QualityOfService

The default quality of service level the system applies to operations the task executes.

var standardInput: Any?

The standard input for the receiver.

var standardOutput: Any?

The standard output for the receiver.

