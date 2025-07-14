

- Shared With You
- SWAttributionView
-  SWAttributionView.BackgroundStyle 

Enumeration

# SWAttributionView.BackgroundStyle

The background styling of the attribution view’s contents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum BackgroundStyle
```

## Topics

### Background styles

case `default`

The default background style the system chooses.

case color

A non-material background color for the view’s contents, best when placed over monochrome backgrounds.

case material

A material background blur for the view’s contents, best when placed over multicolored backgrounds.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the view

enum DisplayContext

The context for the content that influences the ranking of this view’s highlight.

enum HorizontalAlignment

The horizontal alignment of attribution view’s contents.

