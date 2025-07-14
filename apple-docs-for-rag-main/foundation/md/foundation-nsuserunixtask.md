

- Foundation
-  NSUserUnixTask 

Class

# NSUserUnixTask

An object that executes unix applications.

macOS 10.8+

``` source
class NSUserUnixTask
```

## Overview

The NSUserUnixTask class is intended to run unix applications, typically a shell script, from your application. It is intended to execute user-supplied scripts, and will execute them outside of the application’s sandbox, if any.

The class is not intended to execute scripts built into an application; for that, use one of the Process, NSAppleScript, or AMWorkflow classes. If the application is sandboxed, then the script must be in the FileManager.SearchPathDirectory.applicationScriptsDirectory folder. A sandboxed application may read from, but not write to, this folder.

If you simply need to execute unix scripts without regard to input or output, use NSUserScriptTask, which can execute any of the specific types. If you need specific control over the input to, or output from, or the error stream of the script, use this class.

## Topics

### Executing the Unix Script

func execute(withArguments: [String]?, completionHandler: NSUserUnixTask.CompletionHandler?)

Execute the unix script with the specified arguments.

### Standard Unix Streams

var standardError: FileHandle?

The standard error stream.

var standardInput: FileHandle?

The standard input stream.

var standardOutput: FileHandle?

The standard output stream.

### Constants

typealias CompletionHandler

Implement this block to retrieve an error from the Unix scripted executed by execute(withArguments:completionHandler:).

## Relationships

### Inherits From

- NSUserScriptTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Scripts and External Tasks

class Process

An object that represents a subprocess of the current process.

class NSUserScriptTask

An object that executes scripts.

class NSUserAppleScriptTask

An object that executes AppleScript scripts.

class NSUserAutomatorTask

An object that executes Automator workflows.

