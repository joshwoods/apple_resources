

- UIKit
- UIFocusDebugger
-  status() 

Type Method

# status()

Returns the state of the focus system, including information about the currently focused item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func status() -> any UIFocusDebuggerOutput
```

## Return Value

An object the focus debugger uses to output information to the debugger console.

## Discussion

Call this method from the `lldb` debugger using the following command:

- Swift
- Objective-C

```
po UIFocusDebugger.status()
```

```
po [UIFocusDebugger status]
```

The method returns information about the focus system and the currently focused item.

## See Also

### Getting focus information

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

