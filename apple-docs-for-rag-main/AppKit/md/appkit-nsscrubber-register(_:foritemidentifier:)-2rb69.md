

- AppKit
- NSScrubber
-  register(\_:forItemIdentifier:) 

Instance Method

# register(\_:forItemIdentifier:)

Registers a class for the scrubber to use when it creates new items.

macOS 10.12.2+

``` source
@MainActor
func register(
    _ itemViewClass: AnyClass?,
    forItemIdentifier itemIdentifier: NSUserInterfaceItemIdentifier
)
```

## Parameters 

`itemViewClass`  

A class to use for creating items. The class must be descended from NSScrubberItemView. Specify `nil` to unregister a previously registered class.

`itemIdentifier`  

The string that identifies the type of item. You use this string later when requesting new item views. The string must be unique among the other registered item view classes of this scrubber. This parameter must not be an empty string or `nil`.

## See Also

### Creating scrubber items

func register(NSNib?, forItemIdentifier: NSUserInterfaceItemIdentifier)

Registers a nib file for the scrubber to use when it creates new items in the scrubber.

func makeItem(withIdentifier: NSUserInterfaceItemIdentifier, owner: Any?) -> NSScrubberItemView?

Creates or returns a reusable item object with the specified identifier.

