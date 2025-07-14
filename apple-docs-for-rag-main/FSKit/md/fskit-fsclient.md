

- FSKit
-  FSClient 

Class

# FSClient

An interface for apps and daemons to interact with FSKit.

macOS 15.4+

``` source
class FSClient
```

## Overview

FSClient is the primary management interface for FSKit. Use this class to discover FSKit extensions installed on the system, including your own.

Important

Don’t subclass `FSClient`.

## Topics

### Obtaining the shared instance

class var shared: FSClient

The shared instance of the FSKit client class.

### Discovering installed extensions

func fetchInstalledExtensions(completionHandler: ([FSModuleIdentity]?, (any Error)?) -> Void)

Asynchronously retrieves an list of installed file system modules.

class FSModuleIdentity

An installed file system module.

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

