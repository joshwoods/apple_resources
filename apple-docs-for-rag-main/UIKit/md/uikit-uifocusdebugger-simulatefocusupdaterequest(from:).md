

- UIKit
- UIFocusDebugger
-  simulateFocusUpdateRequest(from:) 

Type Method

# simulateFocusUpdateRequest(from:)

Simulates a focus update request from the specified environment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func simulateFocusUpdateRequest(from environment: any UIFocusEnvironment) -> any UIFocusDebuggerOutput
```

## Parameters 

`environment`  

The object you want to generate a request for. Specify the focus system, view, view controller, or window whose state you want. You can also specify any other object that adopts the UIFocusEnvironment protocol.

## Return Value

The UIFocusDebuggerOutput object the focus debugger uses to output the diagnostic information to the debugger console.

## Discussion

Call this method from the `lldb` debugger using the following command. In the example, `obj` corresponds to an object that adopts the UIFocusEnvironment protocol.

- Swift
- Objective-C

```
po UIFocusDebugger.simulateFocusUpdateRequest(from: obj)
```

```
po [UIFocusDebugger simulateFocusUpdateRequestFromEnvironment: obj]
```

The method simulates a focus update request, outlining each step of the process for determining the next focused item.

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

protocol UIFocusDebuggerOutput

An interface for specifying output from a focus debugger object.

