

- Foundation
- NSIndexPath
-  init(forRow:inSection:) 

Initializer

# init(forRow:inSection:)

Initializes an index path with the indexes of a specific row and section in a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    forRow row: Int,
    inSection section: Int
)
```

``` source
convenience init(
    row: Int,
    section: Int
)
```

## Parameters 

`row`  

An index number identifying a row in a UITableView object in a section identified by `section`.

`section`  

An index number identifying a section in a UITableView object.

## Return Value

An NSIndexPath object.

## See Also

### Using Special Node Names

convenience init(forItem: Int, inSection: Int)

Initializes an index path with the indexes of a specific item and section in a collection view.

var section: Int

An index number identifying a section in a table view or collection view.

var row: Int

An index number identifying a row in a section of a table view.

var item: Int

An index number identifying an item in a section of a collection view.

