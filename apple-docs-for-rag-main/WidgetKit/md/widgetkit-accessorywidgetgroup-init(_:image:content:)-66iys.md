

- WidgetKit
- AccessoryWidgetGroup
-  init(\_:image:content:) 

Initializer

# init(\_:image:content:)

Creates an `AccessoryWidgetGroup` that generates its label from a string and image resource.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ title: some StringProtocol,
    image: ImageResource,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label` and `Content` conforms to `View`.

## Parameters 

`title`  

A string for the label of `AccessoryWidgetGroup`.

`image`  

The image resource to lookup.

`content`  

A view builder for the content of the accessory group.

## Discussion

This initializer creates a `Label` view on your behalf, and treats the label similar to `Text/init(_:)-9d1g4`. See `Text` for more information about localizing strings.

