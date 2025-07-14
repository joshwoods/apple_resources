

- SwiftUI
-  LayoutDirection 

Enumeration

# LayoutDirection

A direction in which SwiftUI can lay out content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum LayoutDirection
```

## Overview

SwiftUI supports both left-to-right and right-to-left directions for laying out content to support different languages and locales. The system sets the value based on the user’s locale, but you can also use the environment(_:_:) modifier to override the direction for a view and its child views:

```
MyView()
    .environment(\.layoutDirection, .rightToLeft)
```

You can also read the layoutDirection environment value to find out which direction applies to a particular environment. However, in many cases, you don’t need to take any action based on this value. SwiftUI horizontally flips the x position of each view within its parent, so layout calculations automatically produce the desired effect for both modes without any changes.

## Topics

### Getting layout directions

case leftToRight

A left-to-right layout direction.

case rightToLeft

A right-to-left layout direction.

### Creating a layout direction

init?(UITraitEnvironmentLayoutDirection)

Create a direction from its UITraitEnvironmentLayoutDirection equivalent.

## Relationships

### Conforms To

- CaseIterable
- Equatable
- Hashable
- Sendable

## See Also

### Setting a layout direction

func layoutDirectionBehavior(LayoutDirectionBehavior) -> some View

Sets the behavior of this view for different layout directions.

enum LayoutDirectionBehavior

A description of what should happen when the layout direction changes.

var layoutDirection: LayoutDirection

The layout direction associated with the current environment.

