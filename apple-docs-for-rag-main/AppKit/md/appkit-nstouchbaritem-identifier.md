

- AppKit
- NSTouchBarItem
-  identifier 

Instance Property

# identifier

The identifier for this item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var identifier: NSTouchBarItem.Identifier { get }
```

## Discussion

This read-only property returns the value the item was initialized with.

For all items other than spaces, this value must be globally unique.

## See Also

### Identifying a bar item

struct Identifier

An identifier for an item in the Touch Bar.

