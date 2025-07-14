

- FSKit
-  FSTaskOptions 

Class

# FSTaskOptions

A class that passes command options to a task, optionally providing security-scoped URLs.

macOS 15.4+

``` source
class FSTaskOptions
```

## Topics

### Instance Properties

var taskOptions: [String]

An array of strings that represent command-line options for the task.

### Instance Methods

func url(forOption: String) -> URL?

Retrieves a URL for a given option.

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

class FSTask

A class that enables a file system module to pass log messages and completion notifications to clients.

