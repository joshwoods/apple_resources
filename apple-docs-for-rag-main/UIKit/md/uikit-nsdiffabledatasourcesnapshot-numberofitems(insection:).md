

- UIKit
- NSDiffableDataSourceSnapshot
-  numberOfItems(inSection:) 

Instance Method

# numberOfItems(inSection:)

Returns the number of items in the specified section of the snapshot.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOS

``` source
func numberOfItems(inSection identifier: SectionIdentifierType) -> Int
```

## Parameters 

`identifier`  

The identifier of the section of the snapshot.

## Return Value

The number of items in the specified section. This method returns `0` if the section is empty.

## Discussion

If you call this method with the identifier of a section that doesn’t exist in the snapshot, the app throws an error.

## See Also

### Getting item and section metrics

var numberOfItems: Int

The number of items in the snapshot.

var numberOfSections: Int

The number of sections in the snapshot.

