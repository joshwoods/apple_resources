

- AppKit
- NSScrubber
-  scrollItem(at:to:) 

Instance Method

# scrollItem(at:to:)

Scrolls an item to a specified alignment within the scrubber.

macOS 10.12.2+

``` source
@MainActor
func scrollItem(
    at index: Int,
    to alignment: NSScrubber.Alignment
)
```

## Parameters 

`index`  

The index of the item to be scrolled. Indexes range between `0` and `n-1`, where `n` is the number of items displayed in the scrubber.

`alignment`  

The position the item should be scrolled to. For possible values, see NSScrubber.Alignment. If NSScrubber.Alignment.none, the scrubber scrolls the minimum distance required to make the item visible.

## Discussion

To animate the scroll, call this method on the animator proxy. See NSAnimatablePropertyContainer for details.

