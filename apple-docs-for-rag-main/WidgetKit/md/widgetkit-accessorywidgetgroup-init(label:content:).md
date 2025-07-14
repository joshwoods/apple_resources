

- WidgetKit
- AccessoryWidgetGroup
-  init(label:content:) 

Initializer

# init(label:content:)

Creates an AccessoryWidgetGroup composed of a label and three circular or rounded square contents with equal spacing and vertical alignment.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    @ViewBuilder label: () -> Label,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

## Parameters 

`label`  

A label or a text to show up on the top corner of the widget view to describe the purpose of the group.

`content`  

A view builder for the content of the accessory group.

