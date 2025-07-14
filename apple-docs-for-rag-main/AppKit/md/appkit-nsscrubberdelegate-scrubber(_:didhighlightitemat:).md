

- AppKit
- NSScrubberDelegate
-  scrubber(\_:didHighlightItemAt:) 

Instance Method

# scrubber(\_:didHighlightItemAt:)

Tells the delegate that the item at the specified index was highlighted.

macOS 10.12.2+

``` source
@MainActor
optional func scrubber(
    _ scrubber: NSScrubber,
    didHighlightItemAt highlightedIndex: Int
)
```

## Parameters 

`scrubber`  

The scrubber object that is notifying you of the highlight change.

`highlightedIndex`  

The index of the item that is now highlighted.

## See Also

### Handling item selection and highlighting

func scrubber(NSScrubber, didSelectItemAt: Int)

Tells the delegate that the item at the specified index was selected.

