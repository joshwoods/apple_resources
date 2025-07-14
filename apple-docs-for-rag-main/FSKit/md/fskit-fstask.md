

- FSKit
-  FSTask 

Class

# FSTask

A class that enables a file system module to pass log messages and completion notifications to clients.

macOS 15.4+

``` source
class FSTask
```

## Overview

FSKit creates an instance of this class for each long-running operations.

## Topics

### Logging

func logMessage(String)

Logs the given string to the initiating client.

### Sending completion messages

func didComplete(error: (any Error)?)

Informs the client that the task completed.

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

## See Also

### Tasks

class FSTaskOptions

A class that passes command options to a task, optionally providing security-scoped URLs.

