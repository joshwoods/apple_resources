

- UIKit
- UIPageControl
-  UIPageControl.BackgroundStyle 

Enumeration

# UIPageControl.BackgroundStyle

Constants that define the background styles of the page control.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum BackgroundStyle
```

## Topics

### Constants

case automatic

The default background style, which adapts in response to changes in the page control’s interaction state.

case prominent

The background style that shows a full background regardless of the interaction.

case minimal

The background style that shows a minimal background regardless of the interaction.

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

### Customizing the background style

var backgroundStyle: UIPageControl.BackgroundStyle

The preferred background style.

