

- WidgetKit
- StaticControlConfiguration
-  init(kind:content:) 

Initializer

# init(kind:content:)

Creates a configuration for a control, with no user-configurable options.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
init(
    kind: String,
    @ControlWidgetTemplateBuilder content: @escaping () -> Content
)
```

Available when `Content` conforms to `ControlWidgetTemplate`.

## Parameters 

`kind`  

A string that uniquely identifies the type of control.

`content`  

A template that renders the control.

