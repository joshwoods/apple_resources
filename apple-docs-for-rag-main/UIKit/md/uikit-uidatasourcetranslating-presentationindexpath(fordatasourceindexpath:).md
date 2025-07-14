

- UIKit
- UIDataSourceTranslating
-  presentationIndexPath(forDataSourceIndexPath:) 

Instance Method

# presentationIndexPath(forDataSourceIndexPath:)

Translates an index in your data source object to the equivalent index in your presented layout.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func presentationIndexPath(forDataSourceIndexPath dataSourceIndexPath: IndexPath?) -> IndexPath?
```

**Required**

## Parameters 

`dataSourceIndexPath`  

The index path of an item in the data source object.

## Return Value

The index path of the same item in the presentation layer of your object, or `nil` if the item is not in the presentation layer.

## See Also

### Managing item positions

func dataSourceIndexPath(forPresentationIndexPath: IndexPath?) -> IndexPath?

Translates an index in your presented layout to the equivalent index in your data source object.

**Required**

