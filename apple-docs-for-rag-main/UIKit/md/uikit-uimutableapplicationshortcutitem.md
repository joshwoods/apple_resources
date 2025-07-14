

- UIKit
-  UIMutableApplicationShortcutItem 

Class

# UIMutableApplicationShortcutItem

A mutable Home Screen dynamic quick action, which is an item that specifies a configurable user-initiated action for your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class UIMutableApplicationShortcutItem
```

## Overview

This class is a convenience subclass of UIApplicationShortcutItem, helping you work with registered, and therefore immutable, quick actions. For information about how to use objects of this class in your app, read the overview in UIApplicationShortcutItem.

## Topics

### Inspecting a Home Screen dynamic mutable quick action

var localizedTitle: String

The required, user-visible title for the Home Screen dynamic mutable quick action.

var localizedSubtitle: String?

The optional, user-visible subtitle for the Home Screen dynamic mutable quick action.

var type: String

A required, app-specific string that you can employ to identify the type of quick action to perform.

var icon: UIApplicationShortcutIcon?

The optional icon for the Home Screen dynamic mutable quick action.

var userInfo: [String : any NSSecureCoding]?

Optional, app-specific information that you can provide for use when your app performs the Home Screen dynamic mutable quick action.

### Designating the scene to activate

var targetContentIdentifier: Any?

The object that determines which scene handles the quick action.

## Relationships

### Inherits From

- UIApplicationShortcutItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Home Screen quick actions

Add Home Screen quick actions

Expose commonly used functionality with static or dynamic 3D Touch Home Screen quick actions.

class UIApplicationShortcutItem

An application shortcut item, also called a Home Screen dynamic quick action, that specifies a user-initiated action for your app.

class UIApplicationShortcutIcon

An image you can optionally associate with a Home Screen quick action to improve its appearance and usability.

