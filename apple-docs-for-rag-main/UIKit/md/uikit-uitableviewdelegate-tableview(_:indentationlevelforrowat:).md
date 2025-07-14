

- UIKit
- UITableViewDelegate
-  tableView(\_:indentationLevelForRowAt:) 

Instance Method

# tableView(\_:indentationLevelForRowAt:)

Asks the delegate to return the level of indentation for a row in a given section.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    indentationLevelForRowAt indexPath: IndexPath
) -> Int
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path locating the row in `tableView`.

## Return Value

Returns the depth of the specified row to show its hierarchical position in the section.

## See Also

### Configuring rows for the table view

func tableView(UITableView, willDisplay: UITableViewCell, forRowAt: IndexPath)

Tells the delegate the table view is about to draw a cell for a particular row.

func tableView(UITableView, shouldSpringLoadRowAt: IndexPath, with: any UISpringLoadedInteractionContext) -> Bool

Called to let you fine tune the spring-loading behavior of the rows in a table.

