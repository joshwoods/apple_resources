

- SwiftUI
- NSViewControllerRepresentable
-  updateNSViewController(\_:context:) 

Instance Method

# updateNSViewController(\_:context:)

Updates the state of the specified view controller with new information from SwiftUI.

macOS 10.15+

``` source
@MainActor @preconcurrency
func updateNSViewController(
    _ nsViewController: Self.NSViewControllerType,
    context: Self.Context
)
```

**Required**

## Parameters 

`nsViewController`  

Your custom view controller object.

`context`  

A context structure containing information about the current state of the system.

## Discussion

When the state of your app changes, SwiftUI updates the portions of your interface affected by those changes. SwiftUI calls this method for any changes affecting the corresponding AppKit view controller. Use this method to update the configuration of your view controller to match the new state information provided in the `context` parameter.

## See Also

### Creating and updating the view controller

func makeNSViewController(context: Self.Context) -> Self.NSViewControllerType

Creates the view controller object and configures its initial state.

**Required**

typealias Context

associatedtype NSViewControllerType : NSViewController

The type of view controller to present.

**Required**

