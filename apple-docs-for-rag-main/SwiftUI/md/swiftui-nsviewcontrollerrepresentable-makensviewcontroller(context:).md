

- SwiftUI
- NSViewControllerRepresentable
-  makeNSViewController(context:) 

Instance Method

# makeNSViewController(context:)

Creates the view controller object and configures its initial state.

macOS 10.15+

``` source
@MainActor @preconcurrency
func makeNSViewController(context: Self.Context) -> Self.NSViewControllerType
```

**Required**

## Parameters 

`context`  

A context structure containing information about the current state of the system.

## Return Value

Your AppKit view controller configured with the provided information.

## Discussion

You must implement this method and use it to create your view controller object. Create the view controller using your app’s current data and contents of the `context` parameter. The system calls this method only once, when it creates your view controller for the first time. For all subsequent updates, the system calls the updateNSViewController(_:context:) method.

## See Also

### Creating and updating the view controller

func updateNSViewController(Self.NSViewControllerType, context: Self.Context)

Updates the state of the specified view controller with new information from SwiftUI.

**Required**

typealias Context

associatedtype NSViewControllerType : NSViewController

The type of view controller to present.

**Required**

