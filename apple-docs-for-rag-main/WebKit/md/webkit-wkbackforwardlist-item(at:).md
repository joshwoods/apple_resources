

- WebKit
- WKBackForwardList
-  item(at:) 

Instance Method

# item(at:)

Returns the item at the relative offset from the current item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func item(at index: Int) -> WKBackForwardListItem?
```

## Parameters 

`index`  

The offset of the desired item from the current item. Specify `0` for the current item, `-1` for the immediately preceding item, `1` for the immediately following item, and so on.

## Return Value

The item at the specified offset from the current item, or `nil` if the `index` exceeds the limits of the list.

