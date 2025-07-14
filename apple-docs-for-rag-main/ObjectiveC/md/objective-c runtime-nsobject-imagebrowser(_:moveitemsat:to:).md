

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:moveItemsAt:to:) 

Instance Method

# imageBrowser(\_:moveItemsAt:to:)

Signals that the specified items should be moved to the specified destination.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    moveItemsAt indexes: IndexSet!,
    to destinationIndex: Int
) -> Bool
```

## Parameters 

`aBrowser`  

An image browser view.

`indexes`  

The indexes of the items that should be reordered.

`destinationIndex`  

The starting index of the destination the items should be moved to.

## Return Value

YES if successful; NO otherwise.

## Discussion

This method is optional. It is invoked by the image browser view after Image Kit determines that a reordering operation should be applied. The data source should update itself by reordering its elements.

## See Also

### Related Documentation

@MainActor func setAllowsReordering(_ flag: Bool)

Controls whether the user can reorder items.

