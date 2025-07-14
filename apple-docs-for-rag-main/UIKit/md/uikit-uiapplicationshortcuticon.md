

- UIKit
-  UIApplicationShortcutIcon 

Class

# UIApplicationShortcutIcon

An image you can optionally associate with a Home Screen quick action to improve its appearance and usability.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIApplicationShortcutIcon
```

## Overview

To associate an icon with a quick action, pass it to the quick action item’s initialization method, as described in UIApplicationShortcutItem.

There are three types of quick action icon:

- An icon from a system-provided library of common types, as described in the UIApplicationShortcutIcon.IconType enumeration

- An icon derived from a custom template image in your app’s bundle and preferably in an asset catalog (see Managing assets with asset catalogs)

- An icon representing a contact in the user’s address book, which you access through the Contacts UI framework

## Topics

### Creating a quick action icon

convenience init(type: UIApplicationShortcutIcon.IconType)

Creates a Home Screen quick action icon using a system-defined image.

convenience init(templateImageName: String)

Creates a Home Screen quick action icon based on an image in your app’s bundle, preferably in an asset catalog.

convenience init(systemImageName: String)

Creates a Home Screen quick action icon using a system symbol image.

convenience init(contact: CNContact)

Creates a Home Screen quick action icon from the picture for a contact or a monogram of the contact name if the picture is unavailable.

### Constants

enum IconType

Constants for system-provided icons.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Home Screen quick actions

Add Home Screen quick actions

Expose commonly used functionality with static or dynamic 3D Touch Home Screen quick actions.

class UIApplicationShortcutItem

An application shortcut item, also called a Home Screen dynamic quick action, that specifies a user-initiated action for your app.

class UIMutableApplicationShortcutItem

A mutable Home Screen dynamic quick action, which is an item that specifies a configurable user-initiated action for your app.

