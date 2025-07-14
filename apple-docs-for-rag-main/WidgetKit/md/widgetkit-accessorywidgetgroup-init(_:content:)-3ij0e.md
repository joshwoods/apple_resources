

- WidgetKit
- AccessoryWidgetGroup
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates an `AccessoryWidgetGroup` that generates its label from a string.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ title: some StringProtocol,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

## Parameters 

`title`  

A string for the label of `AccessoryWidgetGroup`.

`content`  

A view builder for the content of the accessory group.

## Discussion

This initializer creates a `Text` view on your behalf, and treats the label similar to `Text/init(_:)-9d1g4`. See `Text` for more information about localizing strings.

