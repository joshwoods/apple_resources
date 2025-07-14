

- User Notifications
- Setting up a remote notification server
-  Setting up broadcast push notifications 

Article

# Setting up broadcast push notifications

Enable broadcast capability for Apple Push Notifications service (APNs).

## Overview

Broadcast push notifications provide an effective way to reach a large audience with Live Activities. Starting in iOS 18 and iPadOS 18, people can subscribe to receive updates on a channel for a Live Activity.

### Determine if your app needs broadcast capability

Instead of using a device token to update a Live Activity for an individual person, you can publish a single broadcast request to APNs to reach everyone interested in receiving an update. This capability removes the need to manage device tokens and send updates to each person with a device token. Broadcast push notifications for Live Activities are effective for updating a multitude of people interested in receiving information about the same activity or event in real time. For example, use broadcast push for flight status updates or sports coverage. When Live Activity updates impact only one person, such as for an order delivery or a ride share, send push notifications directly to the device token. For more information, refer to Sending notification requests to APNs.

Note

Broadcast push notifications are only available on Live Activities.

Tip

Refer to Viewing the status of push notifications using Metrics and APNs.

### Enable broadcast capability

To utilize broadcast capability to power Live Activities for your app, first ensure you have enabled push notifications. For more information on how to enable push notification in your app, refer to Enable push notifications. You can enable Broadcast Capability by signing on to developer.apple.com.

1.  Go to Certificates, IDs & Profiles \> Identifiers

2.  Select the topic you want to enable Broadcast Capability

3.  Enable Broadcast Capability under Push Notifications

To disable broadcast capability, go to the developer portal and unselect the Broadcast Capability, confirm your choice, and Save. Once you delete the capability, APNs deletes all channels and broadcast-related configurations for the topic. You can’t reverse this action: channel IDs are unique every time they’re created, and all the channels in use would be invalidated.

### Examine broadcast push notification metrics

The Overview tab of the Push Notification Console provides comprehensive reports of broadcast push notifications for your app. You can view a four-week history of your application’s broadcast push notification metrics.

Metrics provide information on the number of broadcast push notifications published, the number of devices that received them, and a snapshot count of all devices subscribed to receive broadcast push notifications. The insight you gain from metrics can improve your understanding of usage patterns for Live Activity push notifications. Metrics are collected and aggregated on daily basis.

Important

Metrics only record in the production environment; they aren’t available in the development environment.

The Channels tab provides broadcast push notification metrics for the channels of your app. If you recently deleted a channel, you can still see its metrics in the Push Notifications Console. You can only view a one-week history of your channel’s metrics, and broadcast push notification metrics aren’t displayed for channels with very few subscribers.

The following table describes the metrics for the aggregated broadcast push notification.

| Metric | Description |
|----|----|
| Notifications published | The number of broadcast push notifications accepted by APNs. |
| Notifications delivered | The number of broadcast push notifications delivered by APNs. |
| Total subscriptions | A snapshot count of the device subscriptions. APNs records subscription snapshots throughout the day and reports the highest value for each day. |
| Unique subscribers | Only available for application metrics.  A snapshot count of unique devices subscribed to at least one channel for your app. APNs records subscription snapshots throughout the day and reports the highest value for each day. |

## See Also

### Broadcast push notifications

Sending channel management requests to APNs

Manage channels that your application uses for broadcast push notifications.

Sending broadcast push notification requests to APNs

Transmit your broadcast notification payload to Apple Push Notifications service (APNs).

Handling error responses from Apple Push Notification service

Respond to the status codes returned by APNs servers.

