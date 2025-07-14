

- Foundation
- NSIndexPath
-  section 

Instance Property

# section

An index number identifying a section in a table view or collection view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var section: Int { get }
```

## See Also

### Using Special Node Names

convenience init(forRow: Int, inSection: Int)

Initializes an index path with the indexes of a specific row and section in a table view.

convenience init(forItem: Int, inSection: Int)

Initializes an index path with the indexes of a specific item and section in a collection view.

var row: Int

An index number identifying a row in a section of a table view.

var item: Int

An index number identifying an item in a section of a collection view.

