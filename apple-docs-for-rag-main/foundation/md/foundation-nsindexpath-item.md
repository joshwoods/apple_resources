

- Foundation
- NSIndexPath
-  item 

Instance Property

# item

An index number identifying an item in a section of a collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var item: Int { get }
```

## Discussion

The section the item is in is identified by the value of section.

## See Also

### Using Special Node Names

convenience init(forRow: Int, inSection: Int)

Initializes an index path with the indexes of a specific row and section in a table view.

convenience init(forItem: Int, inSection: Int)

Initializes an index path with the indexes of a specific item and section in a collection view.

var section: Int

An index number identifying a section in a table view or collection view.

var row: Int

An index number identifying a row in a section of a table view.

