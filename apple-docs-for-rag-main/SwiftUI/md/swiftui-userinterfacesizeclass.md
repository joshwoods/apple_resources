

- SwiftUI
-  UserInterfaceSizeClass 

Enumeration

# UserInterfaceSizeClass

A set of values that indicate the visual size available to the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum UserInterfaceSizeClass
```

## Overview

You receive a size class value when you read either the horizontalSizeClass or verticalSizeClass environment value. The value tells you about the amount of space available to your views in a given direction. You can read the size class like any other of the EnvironmentValues, by creating a property with the Environment property wrapper:

```
@Environment(\.horizontalSizeClass) private var horizontalSizeClass
@Environment(\.verticalSizeClass) private var verticalSizeClass
```

SwiftUI sets the size class based on several factors, including:

- The current device type.

- The orientation of the device.

- The appearance of Slide Over and Split View on iPad.

Several built-in views change their behavior based on the size class. For example, a NavigationView presents a multicolumn view when the horizontal size class is UserInterfaceSizeClass.regular, but a single column otherwise. You can also adjust the appearance of custom views by reading the size class and conditioning your views. If you do, be prepared to handle size class changes while your app runs, because factors like device orientation can change at runtime.

## Topics

### Getting size classes

case compact

The compact size class.

case regular

The regular size class.

### Creating a size class

init?(UIUserInterfaceSizeClass)

Creates a SwiftUI size class from the specified UIKit size class.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Reacting to interface characteristics

var isLuminanceReduced: Bool

A Boolean value that indicates whether the display or environment currently requires reduced luminance.

var displayScale: CGFloat

The display scale of this environment.

var pixelLength: CGFloat

The size of a pixel on the screen.

var horizontalSizeClass: UserInterfaceSizeClass?

The horizontal size class of this environment.

var verticalSizeClass: UserInterfaceSizeClass?

The vertical size class of this environment.

