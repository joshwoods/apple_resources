

- SwiftUI
- UIViewControllerRepresentable
-  makeUIViewController(context:) 

Instance Method

# makeUIViewController(context:)

Creates the view controller object and configures its initial state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func makeUIViewController(context: Self.Context) -> Self.UIViewControllerType
```

**Required**

## Parameters 

`context`  

A context structure containing information about the current state of the system.

## Return Value

Your UIKit view controller configured with the provided information.

## Discussion

You must implement this method and use it to create your view controller object. Create the view controller using your app’s current data and contents of the `context` parameter. The system calls this method only once, when it creates your view controller for the first time. For all subsequent updates, the system calls the updateUIViewController(_:context:) method.

## See Also

### Creating and updating the view controller

func updateUIViewController(Self.UIViewControllerType, context: Self.Context)

Updates the state of the specified view controller with new information from SwiftUI.

**Required**

typealias Context

associatedtype UIViewControllerType : UIViewController

The type of view controller to present.

**Required**

