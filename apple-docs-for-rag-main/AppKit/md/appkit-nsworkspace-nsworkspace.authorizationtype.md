

- AppKit
- NSWorkspace
-  NSWorkspace.AuthorizationType 

Enumeration

# NSWorkspace.AuthorizationType

The types of privileged file operations that can be authorized by the user.

macOS 10.14+

``` source
enum AuthorizationType
```

## Overview

To enable your app to prompt the user for these file permissions, you must have a Privileged File Operation entitlement. If you have an app on the Mac App Store or plan to submit your app for review, you can request this entitlement.

## Topics

### Types of Authorization

case createSymbolicLink

Authorization for the app to create a symbolic link.

case replaceFile

Authorization for the app to perform an atomic file write without changing the target file’s permissions.

case setAttributes

Authorization for the app to change specific file attributes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Performing Privileged Operations

func requestAuthorization(to: NSWorkspace.AuthorizationType, completionHandler: (NSWorkspace.Authorization?, (any Error)?) -> Void)

Requests authorization to perform a privileged file operation.

class Authorization

The authorization granted to the app by the user.

