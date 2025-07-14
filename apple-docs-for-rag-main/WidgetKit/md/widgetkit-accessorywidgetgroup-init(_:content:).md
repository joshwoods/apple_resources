

- WidgetKit
- AccessoryWidgetGroup
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates an `AccessoryWidgetGroup` that generates its label from a localized string key.

watchOS 11.0+

``` source
@MainActor @preconcurrency
init(
    _ titleKey: LocalizedStringKey,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Text` and `Content` conforms to `View`.

## Parameters 

`titleKey`  

The key for the `AccessoryWidgetGroup`’s localized label.

`content`  

A view builder for the content of the accessory group.

## Discussion

This initializer creates a `Text` view on your behalf, and treats the localized key similar to `Text/init(_:tableName:bundle:comment:)`. See `Text` for more information about localizing strings.

