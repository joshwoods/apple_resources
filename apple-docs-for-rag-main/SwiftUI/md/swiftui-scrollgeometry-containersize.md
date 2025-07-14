

- SwiftUI
- ScrollGeometry
-  containerSize 

Instance Property

# containerSize

The size of the container of the scroll view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var containerSize: CGSize { get set }
```

## Discussion

This is the overall size of the scroll view. Combining this and the content offset will give you the current visible rect of the scroll view.

