

- Xcode
- Capabilities
-  Configuring Group Activities 

Article

# Configuring Group Activities

Leverage FaceTime infrastructure to create coordinated experiences users can share.

## Overview

Use Group Activities to bring your app’s users together to enjoy new and exciting shared experiences that are built atop SharePlay and the FaceTime infrastructure. For example, a karaoke app might offer karaoke parties where several participants take part simultaneously from their own devices.

Represent shareable activities by creating objects that conform to the GroupActivity protocol and, after a shared activity begins, use GroupSession to synchronize that activity across participants’ devices.

### Add the Group Activities capability to your target

Follow the steps in Add a capability to add the capability to your app’s target, making sure you select the Group Activities capability from Xcode’s Capabilities library. This capability is available on all platforms except watchOS, and you must add it to an app target — Group Activities aren’t available in widgets, extensions, or App Clips.

After you add the Group Activities capability, Xcode updates your target’s entitlements file to include the com.apple.developer.group-session entitlement. If Xcode automatically manages the signing of your app, it also enables Group Activities for your app’s App ID.

Note

If you remove the Group Activities capability in Xcode, you must manually update your App ID’s configuration in your developer account to disable Group Activities.

When you add the Group Activities capability, there are additional steps you must complete before your app’s users can start experiencing shared activities; for more information on these steps, see Defining your app’s SharePlay activities and Joining and managing a shared activity.

## See Also

### Network

Configuring network extensions

Customize the various capabilities of your app’s networking stack, such as proxying DNS queries or creating packet tunnels.

Registering your app with APNs

Communicate with Apple Push Notification service (APNs) and receive a unique device token that identifies your app.

Configuring media device discovery

Add a third-party media device or protocol as a streaming option in the same system menu as AirPlay.

