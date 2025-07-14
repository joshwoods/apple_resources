

- Foundation
- Process
-  environment 

Instance Property

# environment

The environment for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var environment: [String : String]? { get set }
```

## Parameters 

`environmentDictionary`  

A dictionary of environment variable values whose keys are the variable names.

## Discussion

If this method isn’t used, the environment is inherited from the process that created the receiver. This method raises an `NSInvalidArgumentException` if the system has launched the receiver.

## See Also

### Configuring

var arguments: [String]?

The command arguments that the system uses to launch the executable.

var currentDirectoryURL: URL?

The current directory for the receiver.

var executableURL: URL?

The receiver’s executable.

var qualityOfService: QualityOfService

The default quality of service level the system applies to operations the task executes.

var standardError: Any?

The standard error for the receiver.

var standardInput: Any?

The standard input for the receiver.

var standardOutput: Any?

The standard output for the receiver.

