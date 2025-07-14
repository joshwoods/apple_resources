

- CloudKit
- CKNotification
-  init(fromRemoteNotificationDictionary:) 

Initializer

# init(fromRemoteNotificationDictionary:)

Creates a new notification using the specified payload data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init?(fromRemoteNotificationDictionary notificationDictionary: [AnyHashable : Any])
```

## Parameters 

`notificationDictionary`  

The push notification’s payload data. Use the dictionary that the system provides to your app delegate’s application(_:didReceiveRemoteNotification:fetchCompletionHandler:) method. This parameter must not be `nil`.

