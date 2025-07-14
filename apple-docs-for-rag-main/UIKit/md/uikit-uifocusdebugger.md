

- UIKit
-  UIFocusDebugger 

Class

# UIFocusDebugger

A runtime object for debugging focus-related interactions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class UIFocusDebugger
```

## Mentioned in 

Debugging focus issues in your app

## Overview

You do not use this class or its methods directly from your code. During a debugging session, you can call the methods of this class from the `lldb` debugger command line to obtain information about the current state of the focus system.

## Topics

### Getting help

class func help() -> any UIFocusDebuggerOutput

Returns information about how to use the commands of the debugger object.

### Getting focus information

class func status() -> any UIFocusDebuggerOutput

Returns the state of the focus system, including information about the currently focused item.

class func checkFocusability(for: any UIFocusItem) -> any UIFocusDebuggerOutput

Returns information about whether the item can become focused, including any known issues that would prevent the item from becoming focused.

class func focusGroups(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the focus group hierarchy for the specified environment object.

class func preferredFocusEnvironments(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the hierarchy of preferred focus environments for the specified environment object.

class func simulateFocusUpdateRequest(from: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Simulates a focus update request from the specified environment.

protocol UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

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

## See Also

### Focus debugging

Debugging focus issues in your app

Find errors and determine why the next focused item isn’t what you expected.

