

- WidgetKit
- StaticConfiguration
-  init(kind:provider:content:) 

Initializer

# init(kind:provider:content:)

Creates a configuration for a widget, with no user-configurable options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    provider: Provider,
    @ViewBuilder content: @escaping (Provider.Entry) -> Content
) where Provider : TimelineProvider
```

Available when `Content` conforms to `View`.

## Parameters 

`kind`  

A unique string that you choose.

`provider`  

An object that determines the timing of updates to the widget’s views.

`content`  

A view that renders the widget.

## See Also

### Creating a widget configuration

@MainActor @preconcurrency var body: Self.Body { get }

The content and behavior of this widget.

