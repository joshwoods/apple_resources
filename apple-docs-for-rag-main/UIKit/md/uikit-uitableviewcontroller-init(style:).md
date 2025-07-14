

- UIKit
- UITableViewController
-  init(style:) 

Initializer

# init(style:)

Initializes a table view controller to manage a table view of a given style.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(style: UITableView.Style)
```

## Parameters 

`style`  

A constant that specifies the style of table view that the controller object is to manage (UITableView.Style.plain or UITableView.Style.grouped).

## Return Value

An initialized UITableViewController object.

## Discussion

If you use the standard `init` method to initialize a UITableViewController object, a table view in the plain style is created.

## See Also

### Creating a table view controller

init(nibName: String?, bundle: Bundle?)

Creates a table view controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a table view controller from data in an unarchiver.

