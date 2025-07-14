

- UIKit
-  UIFocusDebuggerOutput 

Protocol

# UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
protocol UIFocusDebuggerOutput : NSObjectProtocol
```

## Overview

Don’t use this protocol directly in your code. When debugging your app from the `lldb` command line, the methods of UIFocusDebugger output their results to an object that adopts this protocol. The debugger takes the output and formats it for display.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

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

