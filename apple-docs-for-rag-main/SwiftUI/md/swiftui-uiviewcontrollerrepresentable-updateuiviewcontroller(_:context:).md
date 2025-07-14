

- SwiftUI
- UIViewControllerRepresentable
-  updateUIViewController(\_:context:) 

Instance Method

# updateUIViewController(\_:context:)

Updates the state of the specified view controller with new information from SwiftUI.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func updateUIViewController(
    _ uiViewController: Self.UIViewControllerType,
    context: Self.Context
)
```

**Required**

## Parameters 

`uiViewController`  

Your custom view controller object.

`context`  

A context structure containing information about the current state of the system.

## Discussion

When the state of your app changes, SwiftUI updates the portions of your interface affected by those changes. SwiftUI calls this method for any changes affecting the corresponding UIKit view controller. Use this method to update the configuration of your view controller to match the new state information provided in the `context` parameter.

## See Also

### Creating and updating the view controller

func makeUIViewController(context: Self.Context) -> Self.UIViewControllerType

Creates the view controller object and configures its initial state.

**Required**

typealias Context

associatedtype UIViewControllerType : UIViewController

The type of view controller to present.

**Required**

