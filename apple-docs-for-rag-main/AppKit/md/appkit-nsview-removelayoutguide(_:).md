

- AppKit
- NSView
-  removeLayoutGuide(\_:) 

Instance Method

# removeLayoutGuide(\_:)

Removes the provided layout guide from the view.

macOS 10.11+

``` source
@MainActor
func removeLayoutGuide(_ guide: NSLayoutGuide)
```

## Parameters 

`guide`  

The layout guide to be removed.

## Discussion

This method removes the provided layout guide from the view’s layoutGuides array. It also sets the guide’s owningView property to `nil`. Finally, it removes any constraints to the layout guide.

Layout guides cannot participate in Auto Layout constraints unless they are added by a view in the view hierarchy.

## See Also

### Managing Layout Guides

func addLayoutGuide(NSLayoutGuide)

Adds the provided layout guide to the view.

var layoutGuides: [NSLayoutGuide]

The array of layout guide objects owned by this view.

var layoutMarginsGuide: NSLayoutGuide

A layout guide that provides the recommended amount of padding for content inside of a view.

