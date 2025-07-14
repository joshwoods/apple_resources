

- UIKit
- UIDataSourceTranslating
-  dataSourceIndexPath(forPresentationIndexPath:) 

Instance Method

# dataSourceIndexPath(forPresentationIndexPath:)

Translates an index in your presented layout to the equivalent index in your data source object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func dataSourceIndexPath(forPresentationIndexPath presentationIndexPath: IndexPath?) -> IndexPath?
```

**Required**

## Parameters 

`presentationIndexPath`  

The index path of an item in your presentation layer.

## Return Value

The index path of the same item in the data source object, or `nil` if the item is no longer in the data source.

## See Also

### Managing item positions

func presentationIndexPath(forDataSourceIndexPath: IndexPath?) -> IndexPath?

Translates an index in your data source object to the equivalent index in your presented layout.

**Required**

