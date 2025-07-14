

- Foundation
- NSAttributedString
-  range(of:at:) 

Instance Method

# range(of:at:)

Returns the range of the individual text block that contains the specified location.

macOS 10.0+

``` source
func range(
    of block: NSTextBlock,
    at location: Int
) -> NSRange
```

## Parameters 

`block`  

The text block.

`location`  

The location in the text block.

## Return Value

The range of the text block containing the location.

## See Also

### Calculating ranges for common elements

func itemNumber(in: NSTextList, at: Int) -> Int

Returns the index of the item at the specified location within the list.

func range(of: NSTextList, at: Int) -> NSRange

Returns the range of the specified text list that contains the specified location.

func range(of: NSTextTable, at: Int) -> NSRange

Returns the range of the specified text table that contains the specified location.

