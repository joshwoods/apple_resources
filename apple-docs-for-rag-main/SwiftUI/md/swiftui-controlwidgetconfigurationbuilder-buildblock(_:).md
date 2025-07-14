

- SwiftUI
- ControlWidgetConfigurationBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

Passes a single control widget configuration written as a child control through unmodified.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
static func buildBlock(_ content: Content) -> some ControlWidgetConfiguration where Content : ControlWidgetConfiguration
```

## Discussion

An example of a single control widget configuration written as a child view is `{ StaticControlConfiguration(...) }`.

