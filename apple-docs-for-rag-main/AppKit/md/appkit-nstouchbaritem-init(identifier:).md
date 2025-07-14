

- AppKit
- NSTouchBarItem
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a new item with the specified identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
init(identifier: NSTouchBarItem.Identifier)
```

## Discussion

The designated initializer. The identifier must be globally unique for every item, except for space items.

## See Also

### Creating a bar item

struct Identifier

An identifier for an item in the Touch Bar.

init?(coder: NSCoder)

Initializes and returns a new item from a storyboard or nib file.

