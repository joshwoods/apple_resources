

- UIKit
- UIBarButtonItem
-  UIBarButtonItem.SystemItem 

Enumeration

# UIBarButtonItem.SystemItem

Constants that define system-supplied images for bar button items.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum SystemItem
```

## Topics

### Constants

case done

The system Done button, localized.

case cancel

The system Cancel button, localized.

case edit

The system Edit button, localized.

case save

The system Save button, localized.

case add

The system plus button containing an icon of a plus sign.

case flexibleSpace

Blank space to add between other items.

case fixedSpace

Blank space to add between other items.

case compose

The system compose button.

case reply

The system reply button.

case action

The system action button.

case organize

The system organize button.

case bookmarks

The system bookmarks button.

case search

The system search button.

case refresh

The system refresh button.

case stop

The system stop button.

case camera

The system camera button.

case trash

The system trash button.

case play

The system play button.

case pause

The system pause button.

case rewind

The system rewind button.

case fastForward

The system fast forward button.

case undo

The system undo button.

case redo

The system redo button.

case pageCurl

The system page curl button.

Deprecated

case close

The system close button.

### Enumeration Cases

case writingTools

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating system items

convenience init(systemItem: UIBarButtonItem.SystemItem, primaryAction: UIAction?, menu: UIMenu?)

Creates an item using the specified system item, primary action, and context menu.

convenience init(barButtonSystemItem: UIBarButtonItem.SystemItem, target: Any?, action: Selector?)

Creates an item using the specified system item, target, and action.

