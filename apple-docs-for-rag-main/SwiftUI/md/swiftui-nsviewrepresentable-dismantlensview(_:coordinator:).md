

- SwiftUI
- NSViewRepresentable
-  dismantleNSView(\_:coordinator:) 

Type Method

# dismantleNSView(\_:coordinator:)

Cleans up the presented AppKit view (and coordinator) in anticipation of their removal.

macOS 10.15+

``` source
@MainActor @preconcurrency
static func dismantleNSView(
    _ nsView: Self.NSViewType,
    coordinator: Self.Coordinator
)
```

**Required** Default implementation provided.

## Parameters 

`nsView`  

Your custom view object.

`coordinator`  

The custom coordinator you use to communicate changes back to SwiftUI. If you do not use a custom coordinator instance, the system provides a default instance.

## Discussion

Use this method to perform additional clean-up work related to your custom view. For example, you might use this method to remove observers or update other parts of your SwiftUI interface.

## Default Implementations

### NSViewRepresentable Implementations

static func dismantleNSView(Self.NSViewType, coordinator: Self.Coordinator)

Cleans up the presented AppKit view (and coordinator) in anticipation of their removal.

