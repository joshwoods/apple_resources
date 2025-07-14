

- Foundation
-  NSUserAutomatorTask 

Class

# NSUserAutomatorTask

An object that executes Automator workflows.

macOS 10.8+

``` source
class NSUserAutomatorTask
```

## Overview

The NSUserAutomatorTask class is intended to run Automator workflows from your application. It is intended to execute user-supplied workflows, and will execute them outside of the application’s sandbox, if any.

The class is not intended to execute scripts built into an application; for that, use one of the Process or AMWorkflow classes. If the application is sandboxed, then the script must be in the FileManager.SearchPathDirectory.applicationScriptsDirectory folder. A sandboxed application may read from, but not write to, this folder.

If you simply need to execute scripts without regard to input or output, use NSUserScriptTask, which can execute any of the specific types. If you need specific control over the input to or output from the workflow, use this class.

## Topics

### Executing Automator Tasks

func execute(withInput: (any NSSecureCoding)?, completionHandler: NSUserAutomatorTask.CompletionHandler?)

Execute the Automator workflow by providing it as securely coded input.

var variables: [String : Any]?

The variables required by the Automator workflow.

### Constants

typealias CompletionHandler

Implement this block to retrieve the output of the Automator workflow executed by execute(withInput:completionHandler:).

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

class NSUserUnixTask

An object that executes unix applications.

