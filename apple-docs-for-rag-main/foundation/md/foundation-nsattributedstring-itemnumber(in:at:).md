

- Foundation
- NSAttributedString
-  itemNumber(in:at:) 

Instance Method

# itemNumber(in:at:)

Returns the index of the item at the specified location within the list.

macOS 10.0+

``` source
func itemNumber(
    in list: NSTextList,
    at location: Int
) -> Int
```

## Parameters 

`list`  

The text list.

`location`  

The location of the item.

## Return Value

Returns the index within the list.

## See Also

### Calculating ranges for common elements

func range(of: NSTextBlock, at: Int) -> NSRange

Returns the range of the individual text block that contains the specified location.

func range(of: NSTextList, at: Int) -> NSRange

Returns the range of the specified text list that contains the specified location.

func range(of: NSTextTable, at: Int) -> NSRange

Returns the range of the specified text table that contains the specified location.

