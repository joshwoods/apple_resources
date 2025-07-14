

- SwiftUI
- NSViewControllerRepresentable
-  dismantleNSViewController(\_:coordinator:) 

Type Method

# dismantleNSViewController(\_:coordinator:)

Cleans up the presented view controller (and coordinator) in anticipation of its removal.

macOS 10.15+

``` source
@MainActor @preconcurrency
static func dismantleNSViewController(
    _ nsViewController: Self.NSViewControllerType,
    coordinator: Self.Coordinator
)
```

**Required** Default implementation provided.

## Parameters 

`nsViewController`  

Your custom view controller object.

`coordinator`  

The custom coordinator instance you use to communicate changes back to SwiftUI. If you do not use a custom coordinator, the system provides a default instance.

## Discussion

Use this method to perform additional clean-up work related to your custom view controller. For example, you might use this method to remove observers or update other parts of your SwiftUI interface.

## Default Implementations

### NSViewControllerRepresentable Implementations

static func dismantleNSViewController(Self.NSViewControllerType, coordinator: Self.Coordinator)

Cleans up the presented `NSViewController` (and coordinator) in anticipation of their removal.

