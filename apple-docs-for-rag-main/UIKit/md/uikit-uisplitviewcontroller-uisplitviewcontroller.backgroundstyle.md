

- UIKit
- UISplitViewController
-  UISplitViewController.BackgroundStyle 

Enumeration

# UISplitViewController.BackgroundStyle

Styles that apply a visual effect to the background of a primary view controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum BackgroundStyle
```

## Topics

### Background styles

case none

A style that has no visual effect on the background appearance of the primary view controller.

case sidebar

A style that applies a blurred effect to the background of the primary view controller.

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

### Managing the background style

var primaryBackgroundStyle: UISplitViewController.BackgroundStyle

The background style of the primary view controller.

