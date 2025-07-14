

- SwiftUI
- NSViewRepresentable
-  NSViewType 

Associated Type

# NSViewType

The type of view to present.

macOS 10.15+

``` source
associatedtype NSViewType : NSView
```

**Required**

## See Also

### Creating and updating the view

func makeNSView(context: Self.Context) -> Self.NSViewType

Creates the view object and configures its initial state.

**Required**

func updateNSView(Self.NSViewType, context: Self.Context)

Updates the state of the specified view with new information from SwiftUI.

**Required**

typealias Context

