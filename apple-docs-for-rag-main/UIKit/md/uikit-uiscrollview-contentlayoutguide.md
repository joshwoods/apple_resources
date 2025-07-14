

- UIKit
- UIScrollView
-  contentLayoutGuide 

Instance Property

# contentLayoutGuide

The layout guide based on the untranslated content rectangle of the scroll view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var contentLayoutGuide: UILayoutGuide { get }
```

## Discussion

Use this layout guide when you want to create Auto Layout constraints related to the content area of a scroll view.

## See Also

### Getting the layout guides

var frameLayoutGuide: UILayoutGuide

The layout guide based on the untransformed frame rectangle of the scroll view.

