

- UIKit
- UIView
-  layoutMarginsGuide 

Instance Property

# layoutMarginsGuide

A layout guide representing the view’s margins.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var layoutMarginsGuide: UILayoutGuide { get }
```

## Discussion

Use this layout guide’s anchors to create constraints with the view’s margin.

## See Also

### Related Documentation

var layoutMargins: UIEdgeInsets

The default spacing to use when laying out content in the view.

### Working with layout guides

func addLayoutGuide(UILayoutGuide)

Adds the specified layout guide to the view.

var layoutGuides: [UILayoutGuide]

The array of layout guide objects owned by this view.

var readableContentGuide: UILayoutGuide

A layout guide representing an area with a readable width within the view.

func removeLayoutGuide(UILayoutGuide)

Removes the specified layout guide from the view.

