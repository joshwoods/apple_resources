

- SwiftUI
- NSViewControllerRepresentable
-  NSViewControllerRepresentable.Context 

Type Alias

# NSViewControllerRepresentable.Context

macOS 10.15+

``` source
typealias Context = NSViewControllerRepresentableContext
```

## See Also

### Creating and updating the view controller

func makeNSViewController(context: Self.Context) -> Self.NSViewControllerType

Creates the view controller object and configures its initial state.

**Required**

func updateNSViewController(Self.NSViewControllerType, context: Self.Context)

Updates the state of the specified view controller with new information from SwiftUI.

**Required**

associatedtype NSViewControllerType : NSViewController

The type of view controller to present.

**Required**

