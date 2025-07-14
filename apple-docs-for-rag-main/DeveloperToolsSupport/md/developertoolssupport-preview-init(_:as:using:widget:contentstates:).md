

- DeveloperToolsSupport
- Preview
-  init(\_:as:using:widget:contentStates:) 

Initializer

# init(\_:as:using:widget:contentStates:)

Creates a preview of a live activity widget.

iOS 17.0+iPadOS 17.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    as viewKind: ActivityPreviewViewKind,
    using attributes: Attributes,
    widget: @escaping () -> some Widget,
    @PreviewActivityBuilder contentStates: @escaping @MainActor () async -> [Attributes.ContentState]
) where Attributes : ActivityAttributes
```

## Discussion

The `#Preview` macro expands into a declaration that calls this initializer. To create a preview that appears in the canvas, you must use the macro, not instantiate a Preview directly.

