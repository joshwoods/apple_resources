

- WidgetKit
- AppIntentControlConfiguration
-  init(kind:provider:content:) 

Initializer

# init(kind:provider:content:)

Creates a configuration for a control widget by using a custom intent to provide user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    provider: Provider,
    @ControlWidgetTemplateBuilder content: @escaping (Provider.Value) -> Content
) where Configuration == Provider.Configuration, Provider : AppIntentControlValueProvider
```

Available when `Configuration` conforms to `ControlConfigurationIntent` and `Content` conforms to `ControlWidgetTemplate`.

## Parameters 

`kind`  

A string that uniquely identifies the type of control.

`provider`  

An object that provides a value to the control template. The provider uses your custom intent to prepare this value.

`content`  

A template that renders the control.

