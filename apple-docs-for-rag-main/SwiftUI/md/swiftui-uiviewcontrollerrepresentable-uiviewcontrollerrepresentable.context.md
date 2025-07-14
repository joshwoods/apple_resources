

- SwiftUI
- UIViewControllerRepresentable
-  UIViewControllerRepresentable.Context 

Type Alias

# UIViewControllerRepresentable.Context

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
typealias Context = UIViewControllerRepresentableContext
```

## See Also

### Creating and updating the view controller

func makeUIViewController(context: Self.Context) -> Self.UIViewControllerType

Creates the view controller object and configures its initial state.

**Required**

func updateUIViewController(Self.UIViewControllerType, context: Self.Context)

Updates the state of the specified view controller with new information from SwiftUI.

**Required**

associatedtype UIViewControllerType : UIViewController

The type of view controller to present.

**Required**

