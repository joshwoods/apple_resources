

- UIKit
- UITableView
-  init(frame:style:) 

Initializer

# init(frame:style:)

Creates and returns a table view with the specified frame and style.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    frame: CGRect,
    style: UITableView.Style
)
```

## Parameters 

`frame`  

A rectangle specifying the initial location and size of the table view in its superview’s coordinates. The frame of the table view changes as table cells are added and deleted.

`style`  

A constant that specifies the style of the table view. For a list of valid styles, see UITableView.Style.

## Return Value

Returns an initialized UITableView object.

## Discussion

You must specify the style of a table view when you create it, and you can’t change that style later. If you initialize the table view with the UIView method init(frame:), the UITableView.Style.plain style is used as a default.

## See Also

### Creating a table view

init?(coder: NSCoder)

Creates a table view object from data in an unarchiver.

