

- Foundation
-  NSUserScriptTask 

Class

# NSUserScriptTask

An object that executes scripts.

macOS 10.8+

``` source
class NSUserScriptTask
```

## Overview

The NSUserScriptTask class is able to run all the scripts normally run by the one of its subclasses, however it ignores the results. It is intended to execute user-supplied scripts and will execute them outside of the application’s sandbox, if any.

If you need to execute scripts and get the input and output information use the NSUserUnixTask, NSUserAppleScriptTask, and NSUserAutomatorTask sub classes.

## Topics

### Specifying the Script

init(url: URL) throws

Return a user script task instance given a URL for a script file.

var scriptURL: URL

The URL of the script file.

### Executing the User Script

func execute(completionHandler: NSUserScriptTask.CompletionHandler?)

Executes the script with no input and ignoring any result.

### Constants

typealias CompletionHandler

Implement this block to retrieve the error of the script executed by execute(completionHandler:).

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSUserAppleScriptTask
- NSUserAutomatorTask
- NSUserUnixTask

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

class NSUserAppleScriptTask

An object that executes AppleScript scripts.

class NSUserAutomatorTask

An object that executes Automator workflows.

class NSUserUnixTask

An object that executes unix applications.

