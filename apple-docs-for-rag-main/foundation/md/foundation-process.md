

- Foundation
-  Process 

Class

# Process

An object that represents a subprocess of the current process.

Mac Catalyst 13.0+macOS 10.0+

``` source
class Process
```

## Overview

Using this class, your program can run another program as a subprocess and monitor that program’s execution. Unlike Thread, it doesn’t share memory space with the process that creates it.

A process operates within an environment defined by the current values for several items: the current directory, standard input, standard output, standard error, and the values of any environment variables, inheriting its environment from the process that launches it. If there are any environment variables that should be different for the subprocess (for example, if the current directory needs to change), change it in the instance after initialization, before your app launches it. Your app can’t change a process’s environment while it’s running.

You can only run the subprocess once per instance. Subsequent attempts raise an error.

Important

In a sandboxed app, child processes you create with this class inherit the sandbox of the parent app. Instead, write helper apps as XPC Services because it allows you to specify different sandbox entitlements for helper apps. For more information, see Daemons and Services Programming Guide and XPC.

## Topics

### Creating and Initializing

class func run(URL, arguments: [String], terminationHandler: ((Process) -> Void)?) throws -> Process

Creates and runs a task with a specified executable and arguments.

init()

Returns an initialized process object with the environment of the current process.

### Returning Information

var processIdentifier: Int32

The receiver’s process identifier.

### Running and Stopping

func run() throws

Runs the process with the current environment.

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func resume() -> Bool

Resumes execution of a suspended task.

func suspend() -> Bool

Suspends execution of the receiver task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

func waitUntilExit()

Blocks the process until the receiver is finished.

### Querying the State

var isRunning: Bool

A status that indicates whether the receiver is still running.

var terminationStatus: Int32

The exit status the receiver’s executable returns.

var terminationReason: Process.TerminationReason

The reason the system terminated the task.

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

var standardInput: Any?

The standard input for the receiver.

var standardOutput: Any?

The standard output for the receiver.

### Termination Handler

var terminationHandler: ((Process) -> Void)?

A completion block the system invokes when the task completes.

### Constants

enum TerminationReason

Constants that specify the termination reason values that the system returns.

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

### Notifications

class let didTerminateNotification: NSNotification.Name

Posted when the task has stopped execution.

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

func launch()

Launches the task represented by the receiver.

Deprecated

### Instance Properties

var launchRequirement: LaunchCodeRequirement?

var launchRequirementData: Data?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Scripts and External Tasks

class NSUserScriptTask

An object that executes scripts.

class NSUserAppleScriptTask

An object that executes AppleScript scripts.

class NSUserAutomatorTask

An object that executes Automator workflows.

class NSUserUnixTask

An object that executes unix applications.

