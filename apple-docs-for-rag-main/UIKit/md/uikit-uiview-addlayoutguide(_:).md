

- UIKit
- UIView
-  addLayoutGuide(\_:) 

Instance Method

# addLayoutGuide(\_:)

Adds the specified layout guide to the view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func addLayoutGuide(_ layoutGuide: UILayoutGuide)
```

## Parameters 

`layoutGuide`  

The layout guide to be added.

## Discussion

This method adds the specified layout guide to the end of the view’s layoutGuides array. It also assigns the view to the guide’s owningView property. Each guide can have only one owning view.

After the guide has been added to a view, it can participate in Auto Layout constraints with that view’s hierarchy.

## See Also

### Working with layout guides

var layoutGuides: [UILayoutGuide]

The array of layout guide objects owned by this view.

var layoutMarginsGuide: UILayoutGuide

A layout guide representing the view’s margins.

var readableContentGuide: UILayoutGuide

A layout guide representing an area with a readable width within the view.

func removeLayoutGuide(UILayoutGuide)

Removes the specified layout guide from the view.

