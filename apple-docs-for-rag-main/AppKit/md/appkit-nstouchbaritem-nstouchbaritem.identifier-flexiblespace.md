

- AppKit
- NSTouchBarItem
- NSTouchBarItem.Identifier
-  flexibleSpace 

Type Property

# flexibleSpace

The identifier of an item appropriate for use as a flexible space in a Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
static let flexibleSpace: NSTouchBarItem.Identifier
```

## Discussion

Use this identifier in the itemIdentifiers array on an NSTouchBar object and the system will instantiate the item for you.

## See Also

### Creating identifiers for space items

static let fixedSpaceSmall: NSTouchBarItem.Identifier

The identifier of an item appropriate for use as a small space in a Touch Bar.

static let fixedSpaceLarge: NSTouchBarItem.Identifier

The identifier of an item appropriate for use as a large space in a Touch Bar.

