

- UIKit
- UIView
-  removeLayoutGuide(\_:) 

Instance Method

# removeLayoutGuide(\_:)

Removes the specified layout guide from the view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func removeLayoutGuide(_ layoutGuide: UILayoutGuide)
```

## Parameters 

`layoutGuide`  

The layout guide to be removed.

## Discussion

This method removes the layout guide from the view’s layoutGuides array and sets the guide’s owningView property to `nil`. It also removes any constraints to the layout guide.

Layout guides cannot participate in Auto Layout constraints unless they are added to a view in the view hierarchy.

## See Also

### Working with layout guides

func addLayoutGuide(UILayoutGuide)

Adds the specified layout guide to the view.

var layoutGuides: [UILayoutGuide]

The array of layout guide objects owned by this view.

var layoutMarginsGuide: UILayoutGuide

A layout guide representing the view’s margins.

var readableContentGuide: UILayoutGuide

A layout guide representing an area with a readable width within the view.

