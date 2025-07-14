

- WidgetKit
- IntentConfiguration
-  init(kind:intent:provider:content:) 

Initializer

# init(kind:intent:provider:content:)

Creates a configuration for a widget by using a custom intent definition to provide user-configurable options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    intent: Intent.Type,
    provider: Provider,
    @ViewBuilder content: @escaping (Provider.Entry) -> Content
) where Intent == Provider.Intent, Provider : IntentTimelineProvider
```

Available when `Intent` inherits `INIntent` and `Content` conforms to `View`.

## Parameters 

`kind`  

A unique string that you choose.

`intent`  

A custom intent definition containing user-editable parameters.

`provider`  

An object that determines the timing of updates to the widget’s views.

`content`  

A view that renders the widget.

## See Also

### Creating a widget configuration

@MainActor @preconcurrency var body: Self.Body { get }

The content and behavior of this widget.

