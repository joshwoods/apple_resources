

- SwiftUI
- ControlWidgetTemplateBuilder
-  buildBlock(\_:) 

Type Method

# buildBlock(\_:)

Passes a single control widget template written as a child view through unmodified.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
static func buildBlock(_ content: Content) -> some ControlWidgetTemplate where Content : ControlWidgetTemplate
```

## Discussion

An example of a single control widget template written as a child view is `{ ControlWidgetToggle(...) }`.

