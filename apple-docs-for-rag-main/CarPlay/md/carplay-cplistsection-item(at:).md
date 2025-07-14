

- CarPlay
- CPListSection
-  item(at:) 

Instance Method

# item(at:)

Returns the item at the specified index.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func item(at index: Int) -> any CPListTemplateItem
```

## Parameters 

`index`  

The item’s index in the section.

## Discussion

The index must be within the bounds of the items array, otherwise, your app throws an exception.

## See Also

### Getting Items

var items: [any CPListTemplateItem]

The list of items for the section.

func index(of: any CPListTemplateItem) -> Int

Returns the index of the specified item.

