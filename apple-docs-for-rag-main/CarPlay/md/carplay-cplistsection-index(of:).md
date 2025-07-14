

- CarPlay
- CPListSection
-  index(of:) 

Instance Method

# index(of:)

Returns the index of the specified item.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func index(of item: any CPListTemplateItem) -> Int
```

## Parameters 

`item`  

The item to find in the section.

## Return Value

The item’s index in the section, or NSNotFound if the section doesn’t contain the item.

## See Also

### Getting Items

var items: [any CPListTemplateItem]

The list of items for the section.

func item(at: Int) -> any CPListTemplateItem

Returns the item at the specified index.

