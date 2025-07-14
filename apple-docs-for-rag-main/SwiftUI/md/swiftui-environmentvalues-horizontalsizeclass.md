

- SwiftUI
- EnvironmentValues
-  horizontalSizeClass 

Instance Property

# horizontalSizeClass

The horizontal size class of this environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@backDeployed(before: macOS 14.0, tvOS 17.0, watchOS 10.0)
var horizontalSizeClass: UserInterfaceSizeClass? { get set }
```

## Mentioned in 

Displaying data in lists

## Discussion

You receive a UserInterfaceSizeClass value when you read this environment value. The value tells you about the amount of horizontal space available to the view that reads it. You can read this size class like any other of the EnvironmentValues, by creating a property with the Environment property wrapper:

```
@Environment(\.horizontalSizeClass) private var horizontalSizeClass
```

SwiftUI sets this size class based on several factors, including:

- The current device type.

- The orientation of the device.

- The appearance of Slide Over and Split View on iPad.

Several built-in views change their behavior based on this size class. For example, a NavigationView presents a multicolumn view when the horizontal size class is UserInterfaceSizeClass.regular, but a single column otherwise. You can also adjust the appearance of custom views by reading the size class and conditioning your views. If you do, be prepared to handle size class changes while your app runs, because factors like device orientation can change at runtime.

In watchOS, the horizontal size class is always UserInterfaceSizeClass.compact. In macOS, and tvOS, it’s always UserInterfaceSizeClass.regular.

Writing to the horizontal size class in the environment before macOS 14.0, tvOS 17.0, and watchOS 10.0 is not supported.

## See Also

### Reacting to interface characteristics

var isLuminanceReduced: Bool

A Boolean value that indicates whether the display or environment currently requires reduced luminance.

var displayScale: CGFloat

The display scale of this environment.

var pixelLength: CGFloat

The size of a pixel on the screen.

var verticalSizeClass: UserInterfaceSizeClass?

The vertical size class of this environment.

enum UserInterfaceSizeClass

A set of values that indicate the visual size available to the view.

