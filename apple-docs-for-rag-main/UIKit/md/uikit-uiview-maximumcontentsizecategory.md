

- UIKit
- UIView
-  maximumContentSizeCategory 

Instance Property

# maximumContentSizeCategory

The maximum content size category for the view and its subviews.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var maximumContentSizeCategory: UIContentSizeCategory? { get set }
```

## Discussion

Use this property to limit which content size categories your view hierarchy supports. The limit applies immediately after you set this value and when future content size category updates occur.

Set this property to `nil` to remove the maximum limit for the content size category.

## See Also

### Managing font-sizing preferences

var minimumContentSizeCategory: UIContentSizeCategory?

The minimum content size category for the view and its subviews.

var appliedContentSizeCategoryLimitsDescription: String

A string that lists each of the view’s superviews, its content size category, and whether that view has content size category limits.

