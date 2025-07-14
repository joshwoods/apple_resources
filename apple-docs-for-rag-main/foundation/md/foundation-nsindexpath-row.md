

- Foundation
- NSIndexPath
-  row 

Instance Property

# row

An index number identifying a row in a section of a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
var row: Int { get }
```

## Discussion

The section the row is in is identified by the value of section.

## See Also

### Using Special Node Names

convenience init(forRow: Int, inSection: Int)

Initializes an index path with the indexes of a specific row and section in a table view.

convenience init(forItem: Int, inSection: Int)

Initializes an index path with the indexes of a specific item and section in a collection view.

var section: Int

An index number identifying a section in a table view or collection view.

var item: Int

An index number identifying an item in a section of a collection view.

