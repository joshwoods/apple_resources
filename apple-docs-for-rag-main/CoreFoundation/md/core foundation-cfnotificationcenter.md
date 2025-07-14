

- Core Foundation
-  CFNotificationCenter 

Class

# CFNotificationCenter

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFNotificationCenter
```

## Overview

A CFNotificationCenter object provides the means by which you can send a message, or notification, to any number of recipients, or observers, without having to know anything about the recipients. A notification message consists of a notification name (a CFString), a pointer value that identifies the object posting the notification, and an optional dictionary that contains additional information about the particular notification.

To register as an observer of a notification, you call CFNotificationCenterAddObserver(_:_:_:_:_:_:), providing an identifier for your observer, the callback function that should be called when the notification is posted, and the name of the notification and the object in which you are interested. The observer identifier is passed back to the callback function, along with the notification information. You can use the identifier to distinguish multiple observers using the same callback function. The identifier is also used to unregister the observer with CFNotificationCenterRemoveObserver(_:_:_:_:) and CFNotificationCenterRemoveEveryObserver(_:_:).

To send a notification, you call CFNotificationCenterPostNotification(_:_:_:_:_:), passing in the notification information. The notification center then looks up all the observers that registered for this notification and sends the notification information to their callback functions.

There are three types of CFNotificationCenter—a distributed notification center, a local notification center, and a Darwin notification center—an application may have at most one of each type. The distributed notification is obtained with CFNotificationCenterGetDistributedCenter(). A distributed notification center delivers notifications between applications. In this case, the notification object must always be a CFString object and the notification dictionary must contain only property list values. The local and Darwin notification centers are available in macOS 10.4 and later, and obtained using CFNotificationCenterGetLocalCenter() and CFNotificationCenterGetDarwinNotifyCenter() respectively.

Unlike some other Core Foundation opaque types with names similar to a Cocoa Foundation class (such as CFString and `NSString`), CFNotificationCenter objects cannot be cast (“toll-free bridged”) to NotificationCenter objects or vice-versa.

## Topics

### Accessing a Notification Center

func CFNotificationCenterGetDarwinNotifyCenter() -> CFNotificationCenter!

Returns the application’s Darwin notification center.

func CFNotificationCenterGetDistributedCenter() -> CFNotificationCenter!

Returns the application’s distributed notification center.

func CFNotificationCenterGetLocalCenter() -> CFNotificationCenter!

Returns the application’s local notification center.

### Posting a Notification

func CFNotificationCenterPostNotification(CFNotificationCenter!, CFNotificationName!, UnsafeRawPointer!, CFDictionary!, Bool)

Posts a notification for an object.

func CFNotificationCenterPostNotificationWithOptions(CFNotificationCenter!, CFNotificationName!, UnsafeRawPointer!, CFDictionary!, CFOptionFlags)

Posts a notification for an object using specified options.

### Adding and Removing Observers

func CFNotificationCenterAddObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationCallback!, CFString!, UnsafeRawPointer!, CFNotificationSuspensionBehavior)

Registers an observer to receive notifications.

func CFNotificationCenterRemoveEveryObserver(CFNotificationCenter!, UnsafeRawPointer!)

Stops an observer from receiving any notifications from any object.

func CFNotificationCenterRemoveObserver(CFNotificationCenter!, UnsafeRawPointer!, CFNotificationName!, UnsafeRawPointer!)

Stops an observer from receiving certain notifications.

### Getting the CFNotificationCenter Type ID

func CFNotificationCenterGetTypeID() -> CFTypeID

Returns the type identifier for the CFNotificationCenter opaque type.

### Callbacks

typealias CFNotificationCallback

Callback function invoked for each observer of a notification when the notification is posted.

### Constants

enum CFNotificationSuspensionBehavior

Suspension flags that indicate how distributed notifications should be handled when the receiving application is in the background.

Notification Posting Options

Possible options when posting notifications.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Notification Programming Topics

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

