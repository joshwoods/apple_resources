

- UIKit
- UIFocusDebugger
-  focusGroups(for:) 

Type Method

# focusGroups(for:)

Returns the focus group hierarchy for the specified environment object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func focusGroups(for environment: any UIFocusEnvironment) -> any UIFocusDebuggerOutput
```

## Parameters 

`environment`  

The object you want to generate a focus group hierarchy for. Specify the focus system, view, view controller, or window whose state you want. You can also specify any other object that adopts the UIFocusEnvironment protocol.

## Return Value

An object the focus debugger uses to store the results that it formats for display.

## Discussion

Call this method from the `lldb` debugger using the following command. In the example, `obj` corresponds to an object that adopts the UIFocusEnvironment protocol.

- Swift
- Objective-C

```
po UIFocusDebugger.focusGroups(for: obj)
```

```
po [UIFocusDebugger focusGroupsForEnvironment:obj]
```

The method returns the full hierarchy of focus groups for the focus environment object provided.

Note

This method replaces the `checkFocusGroup(for:)` method, which is functionally equivalent.

## See Also

### Getting focus information

class func status() -> any UIFocusDebuggerOutput

Returns the state of the focus system, including information about the currently focused item.

class func checkFocusability(for: any UIFocusItem) -> any UIFocusDebuggerOutput

Returns information about whether the item can become focused, including any known issues that would prevent the item from becoming focused.

class func preferredFocusEnvironments(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the hierarchy of preferred focus environments for the specified environment object.

class func simulateFocusUpdateRequest(from: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Simulates a focus update request from the specified environment.

protocol UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

