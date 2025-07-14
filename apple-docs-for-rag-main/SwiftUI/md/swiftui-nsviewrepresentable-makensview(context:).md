

- SwiftUI
- NSViewRepresentable
-  makeNSView(context:) 

Instance Method

# makeNSView(context:)

Creates the view object and configures its initial state.

macOS 10.15+

``` source
@MainActor @preconcurrency
func makeNSView(context: Self.Context) -> Self.NSViewType
```

**Required**

## Parameters 

`context`  

A context structure containing information about the current state of the system.

## Return Value

Your AppKit view configured with the provided information.

## Discussion

You must implement this method and use it to create your view object. Configure the view using your app’s current data and contents of the `context` parameter. The system calls this method only once, when it creates your view for the first time. For all subsequent updates, the system calls the updateNSView(_:context:) method.

## See Also

### Creating and updating the view

func updateNSView(Self.NSViewType, context: Self.Context)

Updates the state of the specified view with new information from SwiftUI.

**Required**

typealias Context

associatedtype NSViewType : NSView

The type of view to present.

**Required**

