

- UIKit
- UITableView
-  numberOfRows(inSection:) 

Instance Method

# numberOfRows(inSection:)

Returns the number of rows (table cells) in a specified section.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func numberOfRows(inSection section: Int) -> Int
```

## Parameters 

`section`  

An index number that identifies a section of the table. Table views in a plain style have a section index of zero.

## Return Value

The number of rows in the section.

## Discussion

UITableView gets the value returned by this method from its data source and caches it.

## See Also

### Getting the number of rows and sections

var numberOfSections: Int

The number of sections in the table view.

