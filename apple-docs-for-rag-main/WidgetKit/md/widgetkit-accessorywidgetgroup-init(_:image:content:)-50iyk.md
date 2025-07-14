

- WidgetKit
- AccessoryWidgetGroup
-  init(\_:image:content:) 

Initializer

# init(\_:image:content:)

Creates an `AccessoryWidgetGroup` that generates its label from a localized string key and image resource.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ titleKey: LocalizedStringKey,
    image: ImageResource,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label` and `Content` conforms to `View`.

## Parameters 

`titleKey`  

The key for the `AccessoryWidgetGroup`’s localized label.

`image`  

The image resource to lookup.

`content`  

A view builder for the content of the accessory group.

## Discussion

This initializer creates a `Label` view on your behalf, and treats the localized key similar to `Text/init(_:tableName:bundle:comment:)`. See `Text` for more information about localizing strings.

