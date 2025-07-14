

- AppKit
- NSTouchBarItem
-  NSTouchBarItem.Identifier 

Structure

# NSTouchBarItem.Identifier

An identifier for an item in the Touch Bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
struct Identifier
```

## Topics

### Creating identifiers for space items

static let fixedSpaceSmall: NSTouchBarItem.Identifier

The identifier of an item appropriate for use as a small space in a Touch Bar.

static let fixedSpaceLarge: NSTouchBarItem.Identifier

The identifier of an item appropriate for use as a large space in a Touch Bar.

static let flexibleSpace: NSTouchBarItem.Identifier

The identifier of an item appropriate for use as a flexible space in a Touch Bar.

### Creating identifiers for Touch Bar nesting

static let otherItemsProxy: NSTouchBarItem.Identifier

The identifier of the special “other items proxy”, which is used to nest bars up the responder chain.

### Creating identifiers for multiple choice items

static let candidateList: NSTouchBarItem.Identifier

The standard identifier for a candidate list bar item.

static let characterPicker: NSTouchBarItem.Identifier

The standard identifier for selecting special characters such as Emoji.

### Creating identifiers for text items

static let textFormat: NSTouchBarItem.Identifier

The identifier for a group of text format controls.

static let textAlignment: NSTouchBarItem.Identifier

The identifier for a Touch Bar item used to select the text alignment.

static let textColorPicker: NSTouchBarItem.Identifier

The identifier for a Touch Bar item used to select the text color.

static let textList: NSTouchBarItem.Identifier

The identifier for a Touch Bar item used to control the text list style.

static let textStyle: NSTouchBarItem.Identifier

The identifier for a Touch Bar item used to control the text style.

### Creating a custom identifier

init(String)

Creates an item identifier with the specified custom name.

init(rawValue: String)

Creates an item identifier with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a bar item

init(identifier: NSTouchBarItem.Identifier)

Creates a new item with the specified identifier.

init?(coder: NSCoder)

Initializes and returns a new item from a storyboard or nib file.

