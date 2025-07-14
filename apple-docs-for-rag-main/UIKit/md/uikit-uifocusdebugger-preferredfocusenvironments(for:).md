

- UIKit
- UIFocusDebugger
-  preferredFocusEnvironments(for:) 

Type Method

# preferredFocusEnvironments(for:)

Returns the hierarchy of preferred focus environments for the specified environment object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func preferredFocusEnvironments(for environment: any UIFocusEnvironment) -> any UIFocusDebuggerOutput
```

## Parameters 

`environment`  

The object you want to generate a heirarchy of preferred focus environments for. Specify the focus system, view, view controller, or window whose state you want. You can also specify any other object that adopts the UIFocusEnvironment protocol.

## Return Value

An object the focus debugger uses to store the results to format for display.

## Discussion

Use this method to better understand how the focus system chooses a default focusable item. You call the method from the `lldb` debugger using the following command. In the example, `obj` corresponds to an object that adopts the UIFocusEnvironment protocol.

- Swift
- Objective-C

```
po UIFocusDebugger.preferredFocusEnvironments(for: obj)
```

```
po [UIFocusDebugger preferredFocusEnvironmentsForEnvironment:obj]
```

The method returns the heirarchy of preferred environments for the focus environment object provided.

## See Also

### Getting focus information

class func status() -> any UIFocusDebuggerOutput

Returns the state of the focus system, including information about the currently focused item.

class func checkFocusability(for: any UIFocusItem) -> any UIFocusDebuggerOutput

Returns information about whether the item can become focused, including any known issues that would prevent the item from becoming focused.

class func focusGroups(for: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Returns the focus group hierarchy for the specified environment object.

class func simulateFocusUpdateRequest(from: any UIFocusEnvironment) -> any UIFocusDebuggerOutput

Simulates a focus update request from the specified environment.

protocol UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

