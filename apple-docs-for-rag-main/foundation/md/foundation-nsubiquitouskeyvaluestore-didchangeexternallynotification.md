

- Foundation
- NSUbiquitousKeyValueStore
-  didChangeExternallyNotification 

Type Property

# didChangeExternallyNotification

Posted when the value of one or more keys in the local key-value store changed due to incoming data pushed from iCloud.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let didChangeExternallyNotification: NSNotification.Name
```

## Discussion

This notification is sent only upon a change received from iCloud; it is not sent when your app sets a value.

The user info dictionary can contain the reason for the notification as well as a list of which values changed, as follows:

- The value of the NSUbiquitousKeyValueStoreChangeReasonKey key, when present, indicates why the key-value store changed. Its value is one of the constants in Change Reason Values.

- The value of the NSUbiquitousKeyValueStoreChangedKeysKey, when present, is an array of strings, each the name of a key whose value changed.

The notification object is the NSUbiquitousKeyValueStore object whose contents changed.

Important

Early in your app’s launch sequence, register for the didChangeExternallyNotification notification using the NotificationCenter class. Specify the default key-value store object (obtained using the default class method) as the object whose notifications you want to receive.

