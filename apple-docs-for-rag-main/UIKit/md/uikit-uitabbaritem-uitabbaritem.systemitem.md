

- UIKit
- UITabBarItem
-  UITabBarItem.SystemItem 

Enumeration

# UITabBarItem.SystemItem

Constants that represent the system tab bar items.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum SystemItem
```

## Topics

### System items

case bookmarks

The bookmarks system item.

case contacts

The contacts system item.

case downloads

The downloads system item.

case favorites

The favorites system item.

case featured

The featured system item.

case history

The history system item.

case more

The more system item.

case mostRecent

The most recent system item.

case mostViewed

The most viewed system item.

case recents

The recents system item.

case search

The search system item.

case topRated

The top rated system item.

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

### Creating a tab bar item

convenience init(tabBarSystemItem: UITabBarItem.SystemItem, tag: Int)

Creates a tab bar item using a system-provided configuration.

convenience init(title: String?, image: UIImage?, tag: Int)

Creates a tab bar item that displays a title and an image.

convenience init(title: String?, image: UIImage?, selectedImage: UIImage?)

Creates a tab bar item that toggles the image it displays when its selected state changes.

init()

Creates a tab bar item with a default configuration.

init?(coder: NSCoder)

Creates a tab bar item from a serialized instance.

