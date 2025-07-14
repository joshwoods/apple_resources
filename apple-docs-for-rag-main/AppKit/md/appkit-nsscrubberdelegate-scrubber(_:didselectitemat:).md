

- AppKit
- NSScrubberDelegate
-  scrubber(\_:didSelectItemAt:) 

Instance Method

# scrubber(\_:didSelectItemAt:)

Tells the delegate that the item at the specified index was selected.

macOS 10.12.2+

``` source
@MainActor
optional func scrubber(
    _ scrubber: NSScrubber,
    didSelectItemAt selectedIndex: Int
)
```

## Parameters 

`scrubber`  

The scrubber object that is notifying you of the selection change.

`selectedIndex`  

The index of the item that was selected.

## See Also

### Handling item selection and highlighting

func scrubber(NSScrubber, didHighlightItemAt: Int)

Tells the delegate that the item at the specified index was highlighted.

