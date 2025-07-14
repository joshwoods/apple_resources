

- UIKit
- UITableViewDropDelegate
-  tableView(\_:canHandle:) 

Instance Method

# tableView(\_:canHandle:)

Asks your delegate whether it can accept the specified type of data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    canHandle session: any UIDropSession
) -> Bool
```

## Parameters 

`tableView`  

The table view that’s attempting to handle the drop.

`session`  

The drop session object containing information about the data being dragged.

## Return Value

true if the table view can accept the dragged data, or false if it can’t.

## Mentioned in 

Supporting drag and drop in table views

## Discussion

Implement this method when you want to dynamically determine whether to accept dropped data in your table view. In your implementation, check the type of the dragged data and return a Boolean value indicating whether you can accept the drop. For example, you might call the hasItemsConforming(toTypeIdentifiers:) method of the session object to determine whether it contains data that your app can accept.

If you don’t implement this method, the table view assumes a return value of true. If you return false from this method, the table view doesn’t call any more methods of your drop delegate for the given session.

