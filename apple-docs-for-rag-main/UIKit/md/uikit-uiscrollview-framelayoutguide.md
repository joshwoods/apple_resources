

- UIKit
- UIScrollView
-  frameLayoutGuide 

Instance Property

# frameLayoutGuide

The layout guide based on the untransformed frame rectangle of the scroll view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var frameLayoutGuide: UILayoutGuide { get }
```

## Discussion

Use this layout guide when you want to create Auto Layout constraints that explicitly involve the frame rectangle of the scroll view itself, as opposed to its content rectangle.

## See Also

### Getting the layout guides

var contentLayoutGuide: UILayoutGuide

The layout guide based on the untranslated content rectangle of the scroll view.

