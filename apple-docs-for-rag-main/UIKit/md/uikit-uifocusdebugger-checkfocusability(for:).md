

- UIKit
- UIFocusDebugger
-  checkFocusability(for:) 

Type Method

# checkFocusability(for:)

Returns information about whether the item can become focused, including any known issues that would prevent the item from becoming focused.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func checkFocusability(for item: any UIFocusItem) -> any UIFocusDebuggerOutput
```

## Parameters 

`item`  

The focus item to evaluate.

## Return Value

An object the focus debugger uses to store the results that it will format for display.

## Discussion

Call this method from the `lldb` debugger using the following command. In the example, `item` corresponds to an object that adopts the UIFocusItem protocol.

- Swift
- Objective-C

```
po UIFocusDebugger.checkFocusability(for: item)
```

```
po [UIFocusDebugger checkFocusabilityForItem: item]
```

The method returns the focus-related information, including known issues.

## See Also

### Getting focus information

class func status() -> any UIFocusDebuggerOutput

Returns the state of the focus system, including information about the currently focused item.

class func focusGroups(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the focus group hierarchy for the specified environment object.

class func preferredFocusEnvironments(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the hierarchy of preferred focus environments for the specified environment object.

class func simulateFocusUpdateRequest(from: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Simulates a focus update request from the specified environment.

protocol UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

