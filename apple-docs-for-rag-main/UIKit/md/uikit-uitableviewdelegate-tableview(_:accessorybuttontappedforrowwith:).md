

- UIKit
- UITableViewDelegate
-  tableView(\_:accessoryButtonTappedForRowWith:) 

Instance Method

# tableView(\_:accessoryButtonTappedForRowWith:)

Tells the delegate that the user tapped the detail button for the specified row.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    accessoryButtonTappedForRowWith indexPath: IndexPath
)
```

## Parameters 

`tableView`  

The table view informing the delegate of this event.

`indexPath`  

The index path of the row whose detail button was tapped.

## Mentioned in 

Handling row selection in a table view

## Discussion

Use this method to respond to taps in the detail button accessory view of a row. The table view does not call this method for other types of accessory views.

