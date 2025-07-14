

- UIKit
-  UIPointerLockState 

Class

# UIPointerLockState

An object that contains information about a scene’s pointer lock state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
class UIPointerLockState
```

## Overview

To prevent the pointer from triggering system gestures, for example, bringing up the dock, lock it to your application. Locking the pointer hides the pointer and locks it to just your full-screen application.

## Topics

### Checking the Lock State

var isLocked: Bool

A Boolean value that indicates whether the pointer is locked.

### Updating the Lock State

class let didChangeNotification: NSNotification.Name

A notification that posts when the value of the locked state for a scene changes.

class let sceneUserInfoKey: String

A key that reflects the new locked state.

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

