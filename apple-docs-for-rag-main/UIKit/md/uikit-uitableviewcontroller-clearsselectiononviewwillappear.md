

- UIKit
- UITableViewController
-  clearsSelectionOnViewWillAppear 

Instance Property

# clearsSelectionOnViewWillAppear

A Boolean value indicating if the controller clears the selection when the table appears.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var clearsSelectionOnViewWillAppear: Bool { get set }
```

## Mentioned in 

Handling row selection in a table view

## Discussion

The default value of this property is true. When true, the table view controller clears the table’s current selection when it receives a viewWillAppear(_:) message. Setting this property to false preserves the selection.

