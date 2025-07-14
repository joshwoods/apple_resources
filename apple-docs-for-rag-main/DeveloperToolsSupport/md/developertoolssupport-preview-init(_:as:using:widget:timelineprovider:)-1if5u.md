

- DeveloperToolsSupport
- Preview
-  init(\_:as:using:widget:timelineProvider:) 

Initializer

# init(\_:as:using:widget:timelineProvider:)

Creates a preview of a widget with an `AppIntent` configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    as family: WidgetFamily,
    using intent: Provider.Intent,
    widget: @escaping () -> some Widget,
    timelineProvider: @escaping () -> Provider
) where Provider : AppIntentTimelineProvider
```

## Discussion

The `#Preview` macro expands into a declaration that calls this initializer. To create a preview that appears in the canvas, you must use the macro, not instantiate a Preview directly.

