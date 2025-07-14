

- Foundation
-  NSNotification 

Class

# NSNotification

A container for information broadcast through a notification center to all registered observers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSNotification
```

## Overview

In Swift, this object bridges to Notification; use NSNotification when you need reference semantics or other Foundation-specific behavior.

A notification contains a name, an object, and an optional dictionary, and is broadcast to by instances of NotificationCenter or DistributedNotificationCenter. The name is a tag identifying the notification. The object is any object that the poster of the notification wants to send to observers of that notification (typically, the object posting the notification). The dictionary stores other related objects, if any. NSNotification objects are immutable.

You don’t usually create your own notifications directly, but instead call the NotificationCenter methods post(name:object:) and post(name:object:userInfo:).

Important

The Swift overlay to the Foundation framework provides the Notification structure, which bridges to the NSNotification class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

### Object Comparison

The objects of a notification are compared using pointer equality for local notifications. Distributed notifications use strings as their objects, and those strings are compared using isEqual(_:), because pointer equality doesn’t make sense across process boundaries.

### Creating Subclasses

You can subclass NSNotification to contain information in addition to the notification name, object, and dictionary. This extra data must be agreed upon between notifiers and observers.

NotificationCenter is a class cluster with no instance variables. As such, you must subclass NSNotification and override the primitive methods name, object, and userInfo. You can choose any designated initializer you like, but be sure that your initializer does not call init on `super` (NSNotification is not meant to be instantiated directly, and its `init` method raises an exception).

## Topics

### Creating Notifications

init?(coder: NSCoder)

Initializes a notification with the data from an unarchiver.

convenience init(name: NSNotification.Name, object: Any?)

Returns a new notification object with a specified name and object.

init(name: NSNotification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Initializes a notification with a specified name, object, and user information.

struct Name

A structure that defines the name of a notification.

### Getting Notification Information

var name: NSNotification.Name

The name of the notification.

var object: Any?

The object associated with the notification.

var userInfo: [AnyHashable : Any]?

The user information dictionary associated with the notification.

### Type Properties

static let AVPlayableDidCompleteEnterFullscreen: NSNotification.Name

static let AVPlayableDidCompleteExitFullscreen: NSNotification.Name

static let AVPlayableDidEnterViewingModeImmersive: NSNotification.Name

static let AVPlayableDidEnterViewingModeMono: NSNotification.Name

static let AVPlayableDidEnterViewingModeSpatial: NSNotification.Name

static let AVPlayableDidEnterViewingModeStereo: NSNotification.Name

static let AVPlayableDidPause: NSNotification.Name

static let AVPlayableDidPlay: NSNotification.Name

static let AVPlayableDidShowInfoViewController: NSNotification.Name

static let AVPlayableDidToggleInline: NSNotification.Name

static let AVPlayableDidToggleMuted: NSNotification.Name

static let AVPlayableVideoBoundsDidChange: NSNotification.Name

static let AVPlayableWantsPiPStart: NSNotification.Name

static let AVPlayableWantsPiPStop: NSNotification.Name

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

Notification Programming Topics

