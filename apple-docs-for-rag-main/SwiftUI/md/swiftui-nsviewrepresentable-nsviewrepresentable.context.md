

- SwiftUI
- NSViewRepresentable
-  NSViewRepresentable.Context 

Type Alias

# NSViewRepresentable.Context

macOS 10.15+

``` source
typealias Context = NSViewRepresentableContext
```

## See Also

### Creating and updating the view

func makeNSView(context: Self.Context) -> Self.NSViewType

Creates the view object and configures its initial state.

**Required**

func updateNSView(Self.NSViewType, context: Self.Context)

Updates the state of the specified view with new information from SwiftUI.

**Required**

associatedtype NSViewType : NSView

The type of view to present.

**Required**

