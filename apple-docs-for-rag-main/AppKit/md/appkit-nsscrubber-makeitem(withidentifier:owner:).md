

- AppKit
- NSScrubber
-  makeItem(withIdentifier:owner:) 

Instance Method

# makeItem(withIdentifier:owner:)

Creates or returns a reusable item object with the specified identifier.

macOS 10.12.2+

``` source
@MainActor
func makeItem(
    withIdentifier itemIdentifier: NSUserInterfaceItemIdentifier,
    owner: Any?
) -> NSScrubberItemView?
```

## Parameters 

`itemIdentifier`  

The string that identifies the type of item you want. This is the identifier you specified when registering the item view. The parameter must not be `nil`.

`owner`  

The owner of this item. If the scrubber item is loaded from a nib then this object is set as the nib’s File’s Owner object. Set this parameter to `nil` for scrubber items loaded from classes.

## Return Value

A valid NSScrubberItemView object.

## See Also

### Creating scrubber items

func register(AnyClass?, forItemIdentifier: NSUserInterfaceItemIdentifier)

Registers a class for the scrubber to use when it creates new items.

func register(NSNib?, forItemIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file for the scrubber to use when it creates new items in the scrubber.

