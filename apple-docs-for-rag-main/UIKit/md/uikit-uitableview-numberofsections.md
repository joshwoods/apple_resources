

- UIKit
- UITableView
-  numberOfSections 

Instance Property

# numberOfSections

The number of sections in the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var numberOfSections: Int { get }
```

## Discussion

UITableView gets the value in this property from its data source and caches it.

## See Also

### Getting the number of rows and sections

func numberOfRows(inSection: Int) -> Int

Returns the number of rows (table cells) in a specified section.

