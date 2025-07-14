

- App Store Server Notifications
-  Responding to App Store Server Notifications 

Article

# Responding to App Store Server Notifications

Send HTTP status codes to indicate the success of a notification post.

## Overview

When you set up the endpoints on your server to receive notifications, configure your server to send a response. Use HTTP status codes to indicate whether the App Store server notification post succeeded:

- Send HTTP `200`, or any HTTP code between `200` and `206`, if the post was successful.

- Send HTTP `50x` or `40x` to have the App Store retry the notification, if the post didn’t succeed.

The system considers all other HTTP codes an unsuccessful post. Your server isn’t required to return a data value.

If the App Store server doesn’t receive a success response from your server after the initial notification attempt, it retries as follows:

- For version 2 notifications, it retries five times, at 1, 12, 24, 48, and 72 hours after the previous attempt.

- For version 1 notifications, it retries three times, at 6, 24, and 48 hours after the previous attempt.

Note

Retry notifications are available only in the production environment. In the sandbox environment, the App Store server attempts to send the notification one time.

### Recover from server outages

If your server misses notifications due to an outage, you can always get up-to-date transaction information by calling App Store Server API endpoints including Get Transaction History and Get All Subscription Statuses.

If you use version 2 notifications (App Store Server Notifications V2), you can recover missed notifications by calling Get Notification History. You can also test whether your server is receiving and responding to version 2 notifications correctly by calling the Request a Test Notification endpoint.

## See Also

### Essentials

Enabling App Store Server Notifications

Configure your server and provide an HTTPS URL to receive notifications about in-app purchase events and unreported external purchase tokens.

Receiving App Store Server Notifications

Implement server-side code to receive and parse notification posts.

App Store Server Notifications changelog

Learn about changes to the App Store Server Notifications service.

