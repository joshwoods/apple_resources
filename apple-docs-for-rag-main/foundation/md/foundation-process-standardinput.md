

- Foundation
- Process
-  standardInput 

Instance Property

# standardInput

The standard input for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var standardInput: Any? { get set }
```

## Parameters 

`file`  

The standard input for the receiver, which can be either an FileHandle or an Pipe object.

## Discussion

If `file` is an `NSPipe` object, launching the receiver automatically closes the read end of the pipe in the current task. Don’t create a handle for the pipe and pass that as the argument, or the read end of the pipe won’t be closed automatically.

If this method isn’t used, the standard input is inherited from the process that created the receiver. This method raises an `NSInvalidArgumentException` if the system has lauched the receiver.

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

var standardError: Any?

The standard error for the receiver.

var standardOutput: Any?

The standard output for the receiver.

