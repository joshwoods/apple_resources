

- WidgetKit
- StaticControlConfiguration
-  init(kind:provider:content:) 

Initializer

# init(kind:provider:content:)

Creates a configuration for a control, with no user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    provider: Provider,
    @ControlWidgetTemplateBuilder content: @escaping (Provider.Value) -> Content
) where Provider : ControlValueProvider
```

Available when `Content` conforms to `ControlWidgetTemplate`.

## Parameters 

`kind`  

A string that uniquely identifies the type of control.

`provider`  

An object that provides a value to the control template.

`content`  

A template that renders the control.

