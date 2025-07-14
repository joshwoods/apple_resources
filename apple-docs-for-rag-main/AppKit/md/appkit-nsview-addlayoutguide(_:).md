

- AppKit
- NSView
-  addLayoutGuide(\_:) 

Instance Method

# addLayoutGuide(\_:)

Adds the provided layout guide to the view.

macOS 10.11+

``` source
@MainActor
func addLayoutGuide(_ guide: NSLayoutGuide)
```

## Parameters 

`guide`  

The layout guide to be added.

## Discussion

This method adds the provided layout guide to the end of the view’s layoutGuides array. It also assigns the view to the guide’s owningView property. Each guide can have only one owning view.

After the guide has been added to a view, it can participate in Auto Layout constraints with that view’s hierarchy.

## See Also

### Managing Layout Guides

func removeLayoutGuide(NSLayoutGuide)

Removes the provided layout guide from the view.

var layoutGuides: [NSLayoutGuide]

The array of layout guide objects owned by this view.

var layoutMarginsGuide: NSLayoutGuide

A layout guide that provides the recommended amount of padding for content inside of a view.

