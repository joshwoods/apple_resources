

- AppKit
- NSScrubberFlowLayoutDelegate
-  scrubber(\_:layout:sizeForItemAt:) 

Instance Method

# scrubber(\_:layout:sizeForItemAt:)

Asks the delegate for the size of each item in a scrubber whose items are arranged in a flow layout.

macOS 10.12.2+

``` source
optional func scrubber(
    _ scrubber: NSScrubber,
    layout: NSScrubberFlowLayout,
    sizeForItemAt itemIndex: Int
) -> NSSize
```

## Parameters 

`scrubber`  

The scrubber object displaying the items arranged in a flow layout.

`layout`  

The layout object requesting the information.

`itemIndex`  

The index of the item in the scrubber.

## Return Value

The width and height of the item at the specified index in the scrubber.

