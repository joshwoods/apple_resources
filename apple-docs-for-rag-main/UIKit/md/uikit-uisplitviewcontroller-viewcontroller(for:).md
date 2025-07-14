

- UIKit
- UISplitViewController
-  viewController(for:) 

Instance Method

# viewController(for:)

Returns the view controller associated with the specified column of the split view interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func viewController(for column: UISplitViewController.Column) -> UIViewController?
```

## Parameters 

`column`  

The corresponding column of the split view interface. See UISplitViewController.Column for values.

## Return Value

The corresponding child view controller object.

## Discussion

This method doesn’t apply to classic split view controllers with a style of UISplitViewController.Style.unspecified. For a classic split view controller, instead use the viewControllers property to get the view controllers in the split view interface.

## See Also

### Managing the child view controllers

enum Column

Constants that describe the columns within the split view interface.

func setViewController(UIViewController?, for: UISplitViewController.Column)

Presents the provided view controller in the specified column of the split view interface.

var viewControllers: [UIViewController]

The array of view controllers the split view controller manages.

