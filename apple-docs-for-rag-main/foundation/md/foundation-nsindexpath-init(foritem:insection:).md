

- Foundation
- NSIndexPath
-  init(forItem:inSection:) 

Initializer

# init(forItem:inSection:)

Initializes an index path with the indexes of a specific item and section in a collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
convenience init(
    forItem item: Int,
    inSection section: Int
)
```

**macOS**

``` source
init(
    forItem item: Int,
    inSection section: Int
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
convenience init(
    item: Int,
    section: Int
)
```

## Parameters 

`item`  

An index number identifying an item in a UICollectionView object in a section identified by the `section` parameter.

`section`  

An index number identifying a section in a UICollectionView object.

## Return Value

An NSIndexPath object.

## See Also

### Using Special Node Names

convenience init(forRow: Int, inSection: Int)

Initializes an index path with the indexes of a specific row and section in a table view.

var section: Int

An index number identifying a section in a table view or collection view.

var row: Int

An index number identifying a row in a section of a table view.

var item: Int

An index number identifying an item in a section of a collection view.

