

- WidgetKit
- AppIntentControlConfiguration
-  init(kind:intent:content:) 

Initializer

# init(kind:intent:content:)

Creates a configuration for a control widget by using a custom intent to provide user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    intent: Configuration.Type = Configuration.self,
    @ControlWidgetTemplateBuilder content: @escaping (Configuration) -> Content
)
```

Available when `Configuration` conforms to `ControlConfigurationIntent` and `Content` conforms to `ControlWidgetTemplate`.

## Parameters 

`kind`  

A string that uniquely identifies the type of control.

`intent`  

A custom intent containing user-editable parameters.

`content`  

A template that renders the control.

