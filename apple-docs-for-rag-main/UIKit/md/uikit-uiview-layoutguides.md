

- UIKit
- UIView
-  layoutGuides 

Instance Property

# layoutGuides

The array of layout guide objects owned by this view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var layoutGuides: [UILayoutGuide] { get }
```

## See Also

### Working with layout guides

func addLayoutGuide(UILayoutGuide)

Adds the specified layout guide to the view.

var layoutMarginsGuide: UILayoutGuide

A layout guide representing the view’s margins.

var readableContentGuide: UILayoutGuide

A layout guide representing an area with a readable width within the view.

func removeLayoutGuide(UILayoutGuide)

Removes the specified layout guide from the view.

