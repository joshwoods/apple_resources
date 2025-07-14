

- SwiftUI
- NSViewRepresentable
-  updateNSView(\_:context:) 

Instance Method

# updateNSView(\_:context:)

Updates the state of the specified view with new information from SwiftUI.

macOS 10.15+

``` source
@MainActor @preconcurrency
func updateNSView(
    _ nsView: Self.NSViewType,
    context: Self.Context
)
```

**Required**

## Parameters 

`nsView`  

Your custom view object.

`context`  

A context structure containing information about the current state of the system.

## Discussion

When the state of your app changes, SwiftUI updates the portions of your interface affected by those changes. SwiftUI calls this method for any changes affecting the corresponding AppKit view. Use this method to update the configuration of your view to match the new state information provided in the `context` parameter.

## See Also

### Creating and updating the view

func makeNSView(context: Self.Context) -> Self.NSViewType

Creates the view object and configures its initial state.

**Required**

typealias Context

associatedtype NSViewType : NSView

The type of view to present.

**Required**

