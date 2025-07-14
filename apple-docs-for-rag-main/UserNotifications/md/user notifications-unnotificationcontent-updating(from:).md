

- User Notifications
- UNNotificationContent
-  updating(from:) 

Instance Method

# updating(from:)

Returns a copy of the notification that includes content from the specified provider.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func updating(from provider: any UNNotificationContentProviding) throws -> UNNotificationContent
```

## Parameters 

`provider`  

The notification content providing object.

## Return Value

The notification content object for the content handler.

## Mentioned in 

Implementing communication notifications

## Discussion

The system contextualizes your UNNotificationContent object with other Apple SDK objects conforming to UNNotificationContentProviding. The system specializes the notification and decorates its look and behavior accordingly.

For example, the system treats the notification as a message with an avatar and promotes it to the top of notification center if the object passed in is a valid INSendMessageIntent that conforms to `UNNotificationContentProviding`. The system throws an error with a UNError.Code, if the `UNNotificationContentProviding` object is invalid. Pass the valid `UNNotificationContent` result directly to UNUserNotificationCenter without mutating.

Add this call to the UNNotificationServiceExtension in didReceive(_:withContentHandler:). Your app passes the returned `UNNotificationContent` to the `contentHandler` for incoming push notifications.

