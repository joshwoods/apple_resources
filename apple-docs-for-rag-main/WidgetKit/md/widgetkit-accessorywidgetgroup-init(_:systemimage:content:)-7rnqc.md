

- WidgetKit
- AccessoryWidgetGroup
-  init(\_:systemImage:content:) 

Initializer

# init(\_:systemImage:content:)

Creates an `AccessoryWidgetGroup` that generates its label from a string and system image name.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ titleKey: some StringProtocol,
    systemImage: String,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label` and `Content` conforms to `View`.

## Parameters 

`titleKey`  

A string for the `AccessoryWidgetGroup`’s label.

`systemImage`  

The name of the image resource to lookup.

`content`  

A view builder for the content of the accessory group.

## Discussion

This initializer creates a `Label` view on your behalf, and treats the label similar to `Text/init(_:)-9d1g4`. See `Text` for more information about localizing strings.

