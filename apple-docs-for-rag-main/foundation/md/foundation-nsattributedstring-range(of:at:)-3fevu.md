

- Foundation
- NSAttributedString
-  range(of:at:) 

Instance Method

# range(of:at:)

Returns the range of the specified text table that contains the specified location.

macOS 10.0+

``` source
func range(
    of table: NSTextTable,
    at location: Int
) -> NSRange
```

## Parameters 

`table`  

The text table.

`location`  

The location.

## Return Value

Returns the range of `table` that contains `location`.

## See Also

### Calculating ranges for common elements

func itemNumber(in: NSTextList, at: Int) -> Int

Returns the index of the item at the specified location within the list.

func range(of: NSTextBlock, at: Int) -> NSRange

Returns the range of the individual text block that contains the specified location.

func range(of: NSTextList, at: Int) -> NSRange

Returns the range of the specified text list that contains the specified location.

