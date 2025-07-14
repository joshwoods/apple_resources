

- AppKit
- NSTouchBarItem
- NSTouchBarItem.Identifier
-  otherItemsProxy 

Type Property

# otherItemsProxy

The identifier of the special “other items proxy”, which is used to nest bars up the responder chain.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
static let otherItemsProxy: NSTouchBarItem.Identifier
```

## Discussion

Use this identifier in the itemIdentifiers array of an NSTouchBar object, and a special proxy item will be instantiated for you.

When the NSTouchBar containing this item is visible, bars provided by objects closer to the first responder will be nested inside the space denoted for this item.Note that a touch bar lacking this item identifier will be replaced in its entirety by touch bars closer to the first responder in the responder chain.

