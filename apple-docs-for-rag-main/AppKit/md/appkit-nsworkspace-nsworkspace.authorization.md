

- AppKit
- NSWorkspace
-  NSWorkspace.Authorization 

Class

# NSWorkspace.Authorization

The authorization granted to the app by the user.

macOS 10.14+

``` source
class Authorization
```

## Overview

To enable your app to prompt the user for these file permissions, you must have a Privileged File Operation entitlement. If you have an app on the Mac App Store or plan to submit your app for review, you can request this entitlement.

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

### Performing Privileged Operations

func requestAuthorization(to: NSWorkspace.AuthorizationType, completionHandler: (NSWorkspace.Authorization?, (any Error)?) -> Void)

Requests authorization to perform a privileged file operation.

enum AuthorizationType

The types of privileged file operations that can be authorized by the user.

