

- DeveloperToolsSupport
- Preview
-  init(\_:as:widget:timeline:) 

Initializer

# init(\_:as:widget:timeline:)

Creates a preview of a timeline-style widget.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    as family: WidgetFamily,
    widget: @escaping () -> some Widget,
    @PreviewTimelineBuilder timeline: @escaping @MainActor () async -> [any TimelineEntry]
)
```

## Discussion

The `#Preview` macro expands into a declaration that calls this initializer. To create a preview that appears in the canvas, you must use the macro, not instantiate a Preview directly.

