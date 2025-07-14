

- UIKit
- UISplitViewController
-  init(style:) 

Initializer

# init(style:)

Creates a split view controller with the specified column style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
init(style: UISplitViewController.Style)
```

## Parameters 

`style`  

The split view controller’s style, which describes how many columns the split view controller displays. You can pass in any of the UISplitViewController.Style values except UISplitViewController.Style.unspecified.

## See Also

### Creating a split view controller

init(nibName: String?, bundle: Bundle?)

Creates a split view controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a split view controller from data in an unarchiver.

