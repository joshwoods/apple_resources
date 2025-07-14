

- Foundation
-  NSUserAppleScriptTask 

Class

# NSUserAppleScriptTask

An object that executes AppleScript scripts.

macOS 10.8+

``` source
class NSUserAppleScriptTask
```

## Overview

The NSUserAppleScriptTask class is intended to run AppleScript scripts from your application. It is intended to execute user-supplied scripts and will execute them outside of the application’s sandbox, if any.

The class is not intended to execute scripts built into an application; for that, use one of the Process classes. If the application is sandboxed, then the script must be in the FileManager.SearchPathDirectory.applicationScriptsDirectory folder. A sandboxed application may read from, but not write to, this folder.

If you simply need to execute scripts without regard to input or output, use NSUserScriptTask, which can execute any of the specific types. If you need specific control over the input to or output from the script, use this class.

## Topics

### Executing an AppleScript Script

func execute(withAppleEvent: NSAppleEventDescriptor?, completionHandler: NSUserAppleScriptTask.CompletionHandler?)

Execute the AppleScript script by sending it the specified Apple event.

### Constants

typealias CompletionHandler

Implement this block to retrieve the result of the AppleScript executed by execute(withAppleEvent:completionHandler:).

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

class NSUserAutomatorTask

An object that executes Automator workflows.

class NSUserUnixTask

An object that executes unix applications.

