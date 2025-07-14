

- Foundation
- Process
-  arguments 

Instance Property

# arguments

The command arguments that the system uses to launch the executable.

Mac Catalyst 13.0+macOS 10.0+

``` source
var arguments: [String]? { get set }
```

## Parameters 

`arguments`  

An array of `NSString` objects that supplies the arguments to the task. If `arguments` is `nil`, the system raises an `NSInvalidArgumentException`.

## Discussion

The `NSTask` object converts both `path` and the strings in `arguments` to appropriate C-style strings (using fileSystemRepresentation) before passing them to the task through `argv[]`. The strings in `arguments` don’t undergo shell expansion, so you don’t need to do special quoting, and shell variables, such as `$PWD`, aren’t resolved.

## See Also

### Configuring

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

var standardInput: Any?

The standard input for the receiver.

var standardOutput: Any?

The standard output for the receiver.

